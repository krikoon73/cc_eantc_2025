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

Uptime: 4 days, 18 hours and 37 minutes
Total memory: 8099700 kB
Free memory: 4869064 kB

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
Interface          IP Address         Status       Protocol        MTU  Owner  
------------------ ------------------ ------------ ------------ ------- -------
Ethernet1          20.30.31.30/24     down         down           1500         
Ethernet2          20.30.32.30/24     admin down   down           1500         
Ethernet3          20.30.120.30/24    admin down   down           1500         
Ethernet4          20.30.217.30/24    admin down   down           1500         
Ethernet5          20.30.214.30/24    admin down   down           1500         
Ethernet6          21.30.214.30/24    down         down           1500         
Ethernet7          20.30.184.30/24    up           up             1500         
Ethernet8          21.30.217.30/24    admin down   down           1500         
Ethernet9          20.30.72.30/24     admin down   down           1500         
Ethernet10         21.30.120.30/24    down         down           1500         
Ethernet11         20.30.156.30/24    admin down   down           1500         
Ethernet12         20.30.84.30/24     down         down           1500         
Ethernet13         20.30.53.30/24     down         down           1500         
Ethernet15         20.30.221.30/24    admin down   down           1500         
Ethernet16         21.30.84.30/24     admin down   down           1500         
Ethernet17         20.30.124.30/24    admin down   down           1500         
Ethernet18         21.30.124.30/24    down         down           1500         
Ethernet19         20.30.128.30/24    admin down   down           1500         
Ethernet20         21.30.128.30/24    down         notpresent     1500         
Ethernet21         21.30.156.30/24    admin down   down           1500         
Ethernet29         21.30.32.30/24     admin down   down           1500         
Ethernet31         20.30.66.30/24     up           up             1500         
Ethernet35         20.30.131.30/24    admin down   down           1500         
Ethernet40         20.30.179.30/24    admin down   down           1500         
Ethernet46/1.71    50.10.30.1/24      up           up             1500         
Loopback0          10.0.0.30/32       up           up            65535         
Loopback1000       10.0.30.30/32      up           up            65535         
Loopback5001       10.0.0.30/32       up           up            65535         
Loopback5128       10.128.0.30/32     up           up            65535         
Loopback7001       10.0.30.30/32      up           up            65535         
Management1        192.168.20.30/23   up           up             1500         

```

## show isis neighbors

```text
 
Instance  VRF      System Id        Type Interface          SNPA              State Hold time   Circuit Id          
2-23-5G   default  Ciena-8140-66    L2   Ethernet31         P2P               UP    21          02                  
```

## show isis database detail

```text
Legend:
H - hostname conflict
U - node unreachable

IS-IS Instance: 2-23-5G VRF: default
  IS-IS Level 2 Link State Database
    LSPID                   Seq Num  Cksum  Life Length IS  Received LSPID        Flags
    Arista-PE32-Q2C-32.00-00       916  48928   746    402 L2  0000.0000.0032.00-00  <>
      Remaining lifetime received: 1195 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Arista-PE32-Q2C-32
      Area addresses: 49.0001
      Topology: 2 (IPv6)
      Topology: 0 (IPv4)
      Interface address: 20.32.175.32
      Interface address: 10.0.0.32
      Interface address: 2001:0:32:175::32
      Interface address: 2002::32
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.32.175.175
        IPv4 Interface Address: 20.32.175.32
        Adj-sid: 362170 flags: [L V] weight: 0x0
      IS Neighbor (MT-IPv6): Juniper-175-ACX7100-48L.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:32:175::175
        Global IPv6 Interface Address: 2001:0:32:175::32
        Adj-sid: 362171 flags: [L V F] weight: 0x0
      Reachability         : 20.32.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 10.0.0.32/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 32 Flags: [N] Algorithm: 0
        SR Prefix-SID: 161 Flags: [N] Algorithm: 128
        SR Prefix-SID: 162 Flags: [N] Algorithm: 129
        SR Prefix-SID: 163 Flags: [N] Algorithm: 130
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
    Arrcus-53.00-00            1434  60822   848    502 L2  0000.0000.0053.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Arrcus-53
      Area addresses: 49.0001
      Topology: 0 (IPv4)
      Topology: 2 (IPv6)
      Interface address: 10.0.0.53
      Interface address: 2002::53
      IS Neighbor          : Ciena-8140-66.00    Metric: 10
        IPv4 Neighbor Address: 20.53.66.66
        IPv4 Interface Address: 20.53.66.53
      IS Neighbor          : Ciena-5134-72.00    Metric: 10
        IPv4 Neighbor Address: 20.53.72.72
        IPv4 Interface Address: 20.53.72.53
      IS Neighbor          : H3C_M1A_120.00      Metric: 10
        IPv4 Neighbor Address: 20.53.120.120
        IPv4 Interface Address: 20.53.120.53
      IS Neighbor          : 0000.0000.0124.00   Metric: 10
        IPv4 Neighbor Address: 20.53.124.124
        IPv4 Interface Address: 20.53.124.53
      IS Neighbor          : 0000.0000.0128.00   Metric: 10
        IPv4 Neighbor Address: 20.53.128.128
        IPv4 Interface Address: 20.53.128.53
      IS Neighbor          : Nokia-IXRe2-216.00  Metric: 10
        IPv4 Neighbor Address: 20.53.216.216
        IPv4 Interface Address: 20.53.216.53
      IS Neighbor          : Keysight-185.00     Metric: 10
        IPv4 Neighbor Address: 20.53.185.185
        IPv4 Interface Address: 20.53.185.53
      IS Neighbor (MT-IPv6): Nokia-IXRe2-216.00  Metric: 10
        IPv4 Interface Address: 20.53.216.53
      Reachability         : 20.53.66.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.53.72.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.53.120.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.53.124.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.53.128.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.53.185.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.53.216.0/24 Metric: 10 Type: 1 Up
      Reachability         : 10.0.0.53/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 53 Flags: [N P E] Algorithm: 0
        SR Prefix-SID: 1181 Flags: [N] Algorithm: 128
        SR Prefix-SID: 1182 Flags: [N] Algorithm: 129
        SR Prefix-SID: 1183 Flags: [N] Algorithm: 130
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
    Arrcus-72XC-2-54.00-00       132  65330   773    165 L2  0000.0000.0054.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Arrcus-72XC-2-54
      Area addresses: 49.0001
      Topology: 0 (IPv4)
      Topology: 2 (IPv6)
      Interface address: 10.0.0.54
      IS Neighbor          : Ciena-8140-66.00    Metric: 10
        IPv4 Neighbor Address: 20.54.66.66
        IPv4 Interface Address: 20.54.66.54
      Reachability         : 20.54.66.0/24 Metric: 10 Type: 1 Up
      Reachability         : 10.0.0.54/32 Metric: 10 Type: 1 Up
        SR Prefix-SID: 54 Flags: [N P E] Algorithm: 0
      Router Capabilities: Router Id: 10.0.0.54 Flags: []
        SR Local Block:
          SRLB Base: 16000 Range: 3001
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 10000
        Algorithms:  0
    Ciena-8140-66.00-00         258  19311   920    809 L2  0000.0000.0066.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4)
      Hostname: Ciena-8140-66
      Area addresses: 65.0001
      Topology: 0 (IPv4)
      Interface address: 10.0.0.66
      IS Neighbor          : Arista-Spine3-Q2A-2-23.00 Metric: 10
        IPv4 Neighbor Address: 20.30.66.30
        IPv4 Interface Address: 20.30.66.66
        Adj-sid: 16014 flags: [L V] weight: 0x0
      IS Neighbor          : Juniper-179-ACX7024.00 Metric: 10
        IPv4 Neighbor Address: 20.66.179.179
        IPv4 Interface Address: 20.66.179.66
        Adj-sid: 16013 flags: [L V] weight: 0x0
      IS Neighbor          : Ericsson_84_R6678.00 Metric: 10
        IPv4 Neighbor Address: 20.66.84.84
        IPv4 Interface Address: 20.66.84.66
        Adj-sid: 16017 flags: [L V] weight: 0x0
      IS Neighbor          : Nokia-SXR-214.00    Metric: 10
        IPv4 Neighbor Address: 20.66.214.214
        IPv4 Interface Address: 20.66.214.66
        Adj-sid: 16015 flags: [L V] weight: 0x0
      IS Neighbor          : Arrcus-53.00        Metric: 10
        IPv4 Neighbor Address: 20.53.66.53
        IPv4 Interface Address: 20.53.66.66
        Adj-sid: 16016 flags: [L V] weight: 0x0
      IS Neighbor          : Arrcus-72XC-2-54.00 Metric: 10
        IPv4 Neighbor Address: 20.54.66.54
        IPv4 Interface Address: 20.54.66.66
        Adj-sid: 16018 flags: [L V] weight: 0x0
      IS Neighbor          : Juniper-156-PTX10002-36QDD.00 Metric: 10
        IPv4 Neighbor Address: 20.66.156.156
        IPv4 Interface Address: 20.66.156.66
        Adj-sid: 16019 flags: [L V] weight: 0x0
      Reachability         : 10.0.0.66/32 Metric: 10 Type: 1 Up
        SR Prefix-SID: 66 Flags: [N] Algorithm: 0
      Reachability         : 20.30.66.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.66.84.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.54.66.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.66.179.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.53.66.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.66.214.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.66.156.0/24 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.66 Flags: []
        SR Capability: Flags: [I]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0
    Ciena-5134-72.00-00          82  49033   975    209 L2  0000.0000.0072.00-00  <>
      Remaining lifetime received: 1198 s Modified to: 1200 s
      NLPID: 0xCC(IPv4)
      Hostname: Ciena-5134-72
      Area addresses: 65.0001
      Topology: 0 (IPv4)
      Interface address: 10.0.0.72
      IS Neighbor          : Arrcus-53.00        Metric: 10
        IPv4 Neighbor Address: 20.53.72.53
        IPv4 Interface Address: 20.53.72.72
        Adj-sid: 16004 flags: [L V] weight: 0x0
      Reachability         : 20.53.72.0/24 Metric: 10 Type: 1 Up
      Reachability         : 10.0.0.72/32 Metric: 10 Type: 1 Up
        SR Prefix-SID: 72 Flags: [N] Algorithm: 0
      Router Capabilities: Router Id: 10.0.0.72 Flags: []
        SR Capability: Flags: [I]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0
    Ericsson_84_R6678.00-00        89  34909   944    187 L2  0000.0000.0084.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Ericsson_84_R6678
      Area addresses: 65.0000
      Topology: 0 (IPv4)
      Topology: 2 (IPv6)
      Interface address: 10.0.0.84
      Interface address: 2001:0:66:84::84
      IS Neighbor          : Ciena-8140-66.00    Metric: 10
        IPv4 Interface Address: 20.66.84.84
      Reachability         : 10.0.0.84/32 Metric: 10 Type: 1 Up
        SR Prefix-SID: 84 Flags: [N P] Algorithm: 0
      Reachability (MT-IPv6): 2001:0:66:84::/64 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.84 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  8
        SR Capability: Flags: [I]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0
    H3C_M1A_120.00-00         13915  22798  1194   1239 L2  0000.0000.0120.00-00  <>
      Remaining lifetime received: 13 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: H3C_M1A_120
      Area addresses: 49.0001
      Topology: 0 (IPv4)
      Topology: 2 (IPv6)
      Interface address: 10.0.0.120
      Interface address: 20.53.120.120
      Interface address: 20.120.175.120
      Interface address: 20.120.214.120
      Interface address: 21.120.175.120
      Interface address: 2001:0:120:214::120
      Interface address: 2002::120
      IS Neighbor          : Arrcus-53.00        Metric: 2
        IPv4 Neighbor Address: 20.53.120.53
        IPv4 Interface Address: 20.53.120.120
        Adj-sid: 1147 flags: [L V] weight: 0x0
      IS Neighbor          : Arrcus-53.00        Metric: 2
        IPv4 Neighbor Address: 20.53.120.53
        IPv4 Interface Address: 20.53.120.120
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 1
        IPv4 Neighbor Address: 20.120.175.175
        IPv4 Interface Address: 20.120.175.120
        Adj-sid: 1151 flags: [L V] weight: 0x0
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 1
        IPv4 Neighbor Address: 20.120.175.175
        IPv4 Interface Address: 20.120.175.120
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 2
        IPv4 Neighbor Address: 21.120.175.175
        IPv4 Interface Address: 21.120.175.120
        Adj-sid: 1148 flags: [L V] weight: 0x0
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 2
        IPv4 Neighbor Address: 21.120.175.175
        IPv4 Interface Address: 21.120.175.120
      Reachability         : 10.0.0.120/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 120 Flags: [N] Algorithm: 0
        SR Prefix-SID: 1248 Flags: [N] Algorithm: 128
        SR Prefix-SID: 1249 Flags: [N] Algorithm: 129
        SR Prefix-SID: 1250 Flags: [N] Algorithm: 130
      Reachability         : 20.53.120.0/24 Metric: 2 Type: 1 Up
      Reachability         : 20.120.175.0/24 Metric: 1 Type: 1 Up
      Reachability         : 20.120.214.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.120.217.0/24 Metric: 0 Type: 1 Up
      Reachability         : 21.120.175.0/24 Metric: 2 Type: 1 Up
      Reachability         : 192.168.20.0/23 Metric: 0 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:53:120::/64 Metric: 0 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:120:175::/64 Metric: 0 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:120:214::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:120:217::/64 Metric: 0 Type: 1 Up
      Reachability (MT-IPv6): 2001:1:120:175::/64 Metric: 0 Type: 1 Up
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
    0000.0000.0124.00-00       2067   4938  1177    151 L2  0000.0000.0124.00-00  <>
      Remaining lifetime received: 1198 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Area addresses: 49.0001
      Topology: 0 (IPv4)
      Topology: 2 (IPv6)
      Interface address: 10.0.0.124
      Interface address: 20.53.124.124
      IS Neighbor          : Arrcus-53.00        Metric: 10
        IPv4 Neighbor Address: 20.53.124.53
        IPv4 Interface Address: 20.53.124.124
        Adj-sid: 272 flags: [L V] weight: 0x0
      Reachability         : 10.0.0.124/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 124 Flags: [N P] Algorithm: 0
      Reachability         : 20.53.124.0/24 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.124 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  10
        SR Capability: Flags: [I]
          SRGB Base: 2000 Range: 2001
    0000.0000.0128.00-00       2072  10071   936    151 L2  0000.0000.0128.00-00  <>
      Remaining lifetime received: 1198 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Area addresses: 49.0001
      Topology: 0 (IPv4)
      Topology: 2 (IPv6)
      Interface address: 10.0.0.128
      Interface address: 20.53.128.128
      IS Neighbor          : Arrcus-53.00        Metric: 10
        IPv4 Neighbor Address: 20.53.128.53
        IPv4 Interface Address: 20.53.128.128
        Adj-sid: 48000 flags: [L V] weight: 0x0
      Reachability         : 10.0.0.128/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 128 Flags: [N] Algorithm: 0
      Reachability         : 20.53.128.0/24 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.128 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  10
        SR Capability: Flags: [I]
          SRGB Base: 20000 Range: 2000
    Juniper-131-JCNR.00-00       674  45598   632    338 L2  0000.0000.0131.00-00  <>
      Remaining lifetime received: 1194 s Modified to: 1200 s
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
      Reachability         : 20.131.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 10.0.0.131/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 131 Flags: [N] Algorithm: 0
      Reachability          : 2001:0:131:175::/64 Metric: 10 Type: 1 Up
      Reachability          : fe80::ec97:fbff:fe06:5964/128 Metric: 0 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.131 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  0
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0, 1, 128, 129, 130
      Unsupported TLV: Type: 14 Length: 2
    Juniper-175-ACX7100-48L.00-00      1232  12825   510   1280 L2  0000.0000.0175.00-00  <>
      Remaining lifetime received: 1196 s Modified to: 1200 s
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
      IS Neighbor          : Juniper-179-ACX7024.00 Metric: 1
        IPv4 Neighbor Address: 21.175.179.179
        IPv4 Interface Address: 21.175.179.175
        IPv6 Neighbor Address: 2001:1:175::179:179
        Global IPv6 Interface Address: 2001:1:175::179:175
        Adj-sid: 177 flags: [L V B] weight: 0x0
      IS Neighbor          : Nokia-SR1-217.00    Metric: 10
        IPv4 Neighbor Address: 20.175.217.217
        IPv4 Interface Address: 20.175.217.175
        IPv6 Neighbor Address: 2001:0:175:217::217
        Global IPv6 Interface Address: 2001:0:175:217::175
        Adj-sid: 197 flags: [L V] weight: 0x0
      IS Neighbor          : 221.00              Metric: 10
        IPv4 Neighbor Address: 20.175.221.221
        IPv4 Interface Address: 20.175.221.175
        Global IPv6 Interface Address: 2001:0:175:221::175
        Adj-sid: 199 flags: [L V] weight: 0x0
      IS Neighbor (MT-IPv6): Nokia-SR1-217.00    Metric: 10
        IPv4 Interface Address: 20.175.217.175
        IPv6 Neighbor Address: 2001:0:175:217::217
        Global IPv6 Interface Address: 2001:0:175:217::175
        Adj-sid: 198 flags: [L V F] weight: 0x0
      Reachability         : 127.0.0.1/32 Metric: 0 Type: 1 Up
      Reachability         : 10.0.0.175/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 175 Flags: [N] Algorithm: 0
        SR Prefix-SID: 1305 Flags: [N] Algorithm: 130
        SR Prefix-SID: 1304 Flags: [N] Algorithm: 129
        SR Prefix-SID: 1303 Flags: [N] Algorithm: 128
      Reachability         : 20.66.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.72.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.175.214.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.131.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.32.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 21.175.179.0/24 Metric: 1 Type: 1 Up
      Reachability         : 20.175.179.0/24 Metric: 1 Type: 1 Up
      Reachability         : 20.175.184.0/24 Metric: 10 Type: 1 Up
      Reachability         : 21.120.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.120.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.175.217.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.128.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.175.221.0/24 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2002::175/128 Metric: 0 Type: 1 Up
        SR Prefix-SID: 575 Flags: [N] Algorithm: 0
        SR Prefix-SID: 1705 Flags: [N] Algorithm: 130
        SR Prefix-SID: 1704 Flags: [N] Algorithm: 129
        SR Prefix-SID: 1703 Flags: [N] Algorithm: 128
      Reachability (MT-IPv6): 2001:0:175:214::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:66:175::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:72:175::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:32:175::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:1:175::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:175::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:175:184::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:120:175::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:1:120:175::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:175:217::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:128:175::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:175:221::/64 Metric: 10 Type: 1 Up
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
    Juniper-175-ACX7100-48L.00-01       995   2531   716    299 L2  0000.0000.0175.00-01  <>
      Remaining lifetime received: 1196 s Modified to: 1200 s
      IS Neighbor          : Arista-PE32-Q2C-32.00 Metric: 10
        IPv4 Neighbor Address: 20.32.175.32
        IPv4 Interface Address: 20.32.175.175
        IPv6 Neighbor Address: 2001:0:32:175::32
        Global IPv6 Interface Address: 2001:0:32:175::175
        Adj-sid: 147 flags: [L V] weight: 0x0
      IS Neighbor (MT-IPv6): Arista-PE32-Q2C-32.00 Metric: 10
        IPv4 Interface Address: 20.32.175.175
        IPv6 Neighbor Address: 2001:0:32:175::32
        Global IPv6 Interface Address: 2001:0:32:175::175
        Adj-sid: 148 flags: [L V F] weight: 0x0
    Juniper-175-ACX7100-48L.00-02       675   4392   873    434 L2  0000.0000.0175.00-02  <>
      Remaining lifetime received: 1196 s Modified to: 1200 s
      IS Neighbor          : Juniper-179-ACX7024.00 Metric: 1
        IPv4 Neighbor Address: 20.175.179.179
        IPv4 Interface Address: 20.175.179.175
        IPv6 Neighbor Address: 2001:0:175::179:179
        Global IPv6 Interface Address: 2001:0:175::179:175
        Adj-sid: 187 flags: [L V B] weight: 0x0
      IS Neighbor          : H3C_M1A_120.00      Metric: 10
        IPv4 Neighbor Address: 21.120.175.120
        IPv4 Interface Address: 21.120.175.175
        Global IPv6 Interface Address: 2001:1:120:175::175
        Adj-sid: 195 flags: [L V] weight: 0x0
      IS Neighbor          : H3C_M1A_120.00      Metric: 10
        IPv4 Neighbor Address: 20.120.175.120
        IPv4 Interface Address: 20.120.175.175
        Global IPv6 Interface Address: 2001:0:120:175::175
        Adj-sid: 194 flags: [L V] weight: 0x0
      Reachability (MT-IPv6): 2001:0:131:175::/64 Metric: 10 Type: 1 Up
 H  Juniper-179-ACX7024.00-00       879   3953  1007    464 L2  0000.0000.0179.00-00  <>
      Remaining lifetime received: 1194 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Juniper-179-ACX7024
      Area addresses: 49.0001
      Interface address: 10.0.0.179
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.175.179.175
        IPv4 Interface Address: 20.175.179.179
        IPv6 Neighbor Address: 2001:0:175::179:175
        Global IPv6 Interface Address: 2001:0:175::179:179
        Adj-sid: 29 flags: [L V F] weight: 0x0
        Adj-sid: 28 flags: [L V] weight: 0x0
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 21.175.179.175
        IPv4 Interface Address: 21.175.179.179
        IPv6 Neighbor Address: 2001:1:175::179:175
        Global IPv6 Interface Address: 2001:1:175::179:179
        Adj-sid: 26 flags: [L V F] weight: 0x0
        Adj-sid: 25 flags: [L V] weight: 0x0
      Reachability         : 10.0.0.179/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 179 Flags: [N] Algorithm: 0
        SR Prefix-SID: 1307 Flags: [N] Algorithm: 128
        SR Prefix-SID: 1308 Flags: [N] Algorithm: 129
        SR Prefix-SID: 1309 Flags: [N] Algorithm: 130
      Router Capabilities: Router Id: 10.0.0.179 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  8
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0, 1, 128, 129, 130
      Unsupported TLV: Type: 14 Length: 2
    Nokia-SXR-214.00-00       24158  55527  1190    257 L2  0000.0000.0214.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Nokia-SXR-214
      Area addresses: 49.0001
      Topology: 0 (IPv4)
      Topology: 2 (IPv6)
      Interface address: 10.0.0.214
      Interface address: 20.66.214.214
      Interface address: 2000::214
      Interface address: 2001:0:66:214::214
      IS Neighbor          : Ciena-8140-66.00    Metric: 10
        IPv4 Neighbor Address: 20.66.214.66
        IPv4 Interface Address: 20.66.214.214
        Adj-sid: 30045 flags: [L V B] weight: 0x0
      Reachability         : 20.66.214.0/24 Metric: 10 Type: 1 Up
      Reachability         : 10.0.0.214/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 214 Flags: [N P] Algorithm: 0
      Reachability (MT-IPv6): 2000::214/128 Metric: 0 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:66:214::/64 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.214 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  15
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0
    Arista-Spine3-Q2A-2-23.00-00        92  26037   636    167 L2  0000.0000.3030.00-00  <>
      LSP generation remaining wait time: 0 ms
      Time remaining until refresh: 336 s
      NLPID: 0xCC(IPv4)
      Hostname: Arista-Spine3-Q2A-2-23
      Area addresses: 49.0001
      Interface address: 10.0.30.30
      Interface address: 20.30.66.30
      IS Neighbor          : Ciena-8140-66.00    Metric: 1
        IPv4 Neighbor Address: 20.30.66.66
        IPv4 Interface Address: 20.30.66.30
        Adj-sid: 378674 flags: [L V] weight: 0x0
      Reachability         : 10.0.30.30/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 330 Flags: [N] Algorithm: 0
      Reachability         : 20.30.66.0/24 Metric: 1 Type: 1 Up
      Router Capabilities: Router Id: 10.0.30.30 Flags: []
        SR Local Block:
          SRLB Base: 965536 Range: 65536
        Area leader priority: 250 algorithm: 0
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  12
        SR Capability: Flags: [I]
          SRGB Base: 20000 Range: 2000
    Juniper-156-PTX10002-36QDD.00-00       107  49284   815    291 L2  0000.0001.0156.00-00  <>
      Remaining lifetime received: 1198 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Juniper-156-PTX10002-36QDD
      Area addresses: 49.0001
      Interface address: 10.0.0.156
      Interface address: 10.0.1.156
      Interface address: 2002::156
      IS Neighbor          : Nokia-IXRe2-216.00  Metric: 10
        IPv4 Neighbor Address: 20.156.216.216
        IPv4 Interface Address: 20.156.216.156
        Adj-sid: 28 flags: [L V] weight: 0x0
      IS Neighbor          : Ciena-8140-66.00    Metric: 10
        IPv4 Neighbor Address: 20.66.156.66
        IPv4 Interface Address: 20.66.156.156
        Adj-sid: 29 flags: [L V] weight: 0x0
      Reachability         : 10.0.1.156/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 456 Flags: [N] Algorithm: 0
      Router Capabilities: Router Id: 10.0.0.156 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  0
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0, 1
      Unsupported TLV: Type: 14 Length: 2
 H  Juniper-179-ACX7024.00-00       567  25367   953    222 L2  0000.0001.0179.00-00  <>
      Remaining lifetime received: 1198 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Juniper-179-ACX7024
      Area addresses: 49.0001
      Interface address: 10.0.0.179
      Interface address: 10.0.1.179
      IS Neighbor          : Ciena-8140-66.00    Metric: 10
        IPv4 Neighbor Address: 20.66.179.66
        IPv4 Interface Address: 20.66.179.179
        Adj-sid: 31 flags: [L V] weight: 0x0
      Reachability         : 10.0.1.179/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 479 Flags: [N] Algorithm: 0
      Router Capabilities: Router Id: 10.0.0.179 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  8
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0, 1
      Unsupported TLV: Type: 14 Length: 2
    Nokia-IXRe2-216.00-00      1848  43736  1111    322 L2  0100.0000.0216.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Nokia-IXRe2-216
      Area addresses: 49.0001.0000.0000.0216.00
      Topology: 0 (IPv4)
      Topology: 2 (IPv6)
      Interface address: 10.0.0.216
      Interface address: 20.53.216.216
      Interface address: 20.156.216.216
      Interface address: 2001:0:53:216::216
      Interface address: 2002::216
      IS Neighbor          : Arrcus-53.00        Metric: 10
        IPv4 Neighbor Address: 20.53.216.53
        IPv4 Interface Address: 20.53.216.216
        Adj-sid: 1048574 flags: [L V B] weight: 0x0
      IS Neighbor          : Juniper-156-PTX10002-36QDD.00 Metric: 10
        IPv4 Neighbor Address: 20.156.216.156
        IPv4 Interface Address: 20.156.216.216
        Adj-sid: 1048572 flags: [L V B] weight: 0x0
      IS Neighbor (MT-IPv6): Arrcus-53.00        Metric: 10
      Reachability         : 20.53.216.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.156.216.0/24 Metric: 10 Type: 1 Up
      Reachability         : 10.0.0.216/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 216 Flags: [N P] Algorithm: 0
      Reachability (MT-IPv6): 2001:0:53:216::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2002::216/128 Metric: 0 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.216 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  11
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0
    Nokia-SR1-217.00-00        1285  45905   622    392 L2  0100.0000.0217.00-00  <>
      Remaining lifetime received: 1196 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Nokia-SR1-217
      Area addresses: 49.0001.0000.0000.0217.00
      Topology: 0 (IPv4)
      Topology: 2 (IPv6)
      Interface address: 10.0.0.217
      Interface address: 20.175.217.217
      Interface address: 2001:0:175:217::217
      Interface address: 2002::217
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.175.217.175
        IPv4 Interface Address: 20.175.217.217
        Adj-sid: 524268 flags: [L V B] weight: 0x0
      IS Neighbor (MT-IPv6): Juniper-175-ACX7100-48L.00 Metric: 10
      Reachability         : 10.0.0.217/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 57 Flags: [N P] Algorithm: 0
        SR Prefix-SID: 1345 Flags: [N P] Algorithm: 128
        SR Prefix-SID: 1346 Flags: [N P] Algorithm: 129
        SR Prefix-SID: 1347 Flags: [N P] Algorithm: 130
      Reachability         : 20.175.217.0/24 Metric: 10 Type: 1 Up
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
    221.00-00                   860  59290  1118     86 L2  0221.0221.0221.00-00  <>
      Remaining lifetime received: 1196 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Area addresses: 49.0001
      Router Capabilities: Router Id: 10.0.0.221 Flags: []
        SR Local Block:
          SRLB Base: 626688 Range: 14336
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  10
        SR Capability: Flags: [I]
          SRGB Base: 720000 Range: 2000
        Algorithms:  0, 128, 129, 130
      Unsupported TLV: Type: 14 Length: 2
    221.00-01                    90  11242  1194     32 L2  0221.0221.0221.00-01  <>
      Remaining lifetime received: 1196 s Modified to: 1200 s
      Hostname: 221
    221.00-02                   607  14667  1004    305 L2  0221.0221.0221.00-02  <>
      Remaining lifetime received: 1196 s Modified to: 1200 s
      Interface address: 10.0.0.221
      Interface address: 20.175.221.221
      Interface address: 1221::1
      Interface address: 2001:0:175:221::221
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.175.221.175
        IPv4 Interface Address: 20.175.221.221
        Adj-sid: 524293 flags: [L V B] weight: 0x0
        Adj-sid: 524290 flags: [L V] weight: 0x0
      Reachability         : 10.0.0.221/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 221 Flags: [N] Algorithm: 0
        SR Prefix-SID: 1349 Flags: [N] Algorithm: 128
        SR Prefix-SID: 1350 Flags: [N] Algorithm: 129
        SR Prefix-SID: 1351 Flags: [N] Algorithm: 130
      Reachability         : 20.175.221.0/24 Metric: 10 Type: 1 Up
      Reachability          : 1221::1/128 Metric: 0 Type: 1 Up
      Reachability          : 2001:0:175:221::/64 Metric: 10 Type: 1 Up
    Keysight-185.00-00            8   8805   753    132 L2  6500.0000.0185.00-00  <DefaultAtt>
      Remaining lifetime received: 1195 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6) 0x81(CLNP)
      Hostname: Keysight-185
      Area addresses: 49.0001
      Interface address: 20.53.185.185
      IS Neighbor          : Arrcus-53.00        Metric: 10
        Adj-sid: 9001 flags: [L V] weight: 0x0
      Reachability         : 10.0.0.185/32 Metric: 10 Type: 1 Up
        SR Prefix-SID: 185 Flags: [N] Algorithm: 0
      Reachability         : 20.53.185.0/24 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.185 Flags: []
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0

Legend:
H - hostname conflict
U - node unreachable

IS-IS Instance: IGP VRF: default
  IS-IS Level 2 Link State Database
    LSPID                   Seq Num  Cksum  Life Length IS  Received LSPID        Flags
    Arista-Spine3-Q2A-30.00-00      6990  51392   739    313 L2  0000.0000.0030.00-00  <>
      LSP generation remaining wait time: 0 ms
      Time remaining until refresh: 439 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Arista-Spine3-Q2A-30
      Area addresses: 49.0001
      Topology: 2 (IPv6)
      Topology: 0 (IPv4)
      Interface address: 10.0.0.30
      Interface address: 20.30.184.30
      Interface address: 2002::30
      Interface address: 2001:0:30:184::30
      Reachability         : 10.0.0.30/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 30 Flags: [N] Algorithm: 0
        SR Prefix-SID: 158 Flags: [N] Algorithm: 128
        SR Prefix-SID: 159 Flags: [N] Algorithm: 129
        SR Prefix-SID: 160 Flags: [N] Algorithm: 130
      Reachability         : 20.30.184.0/24 Metric: 1 Type: 1 Up
      Reachability (MT-IPv6): 2002::30/128 Metric: 10 Type: 1 Up
        SR Prefix-SID: 430 Flags: [N] Algorithm: 0
        SR Prefix-SID: 558 Flags: [N] Algorithm: 128
        SR Prefix-SID: 559 Flags: [N] Algorithm: 129
        SR Prefix-SID: 560 Flags: [N] Algorithm: 130
      Reachability (MT-IPv6): 2001:0:30:184::/64 Metric: 10 Type: 1 Up
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

```

## show isis database traffic-engineering

```text
Legend:
H - hostname conflict
U - node unreachable

IS-IS Instance: 2-23-5G VRF: default
  IS-IS Level 2 Link State Database
    LSPID                   Seq Num  Cksum  Life Length IS  Received LSPID        Flags
    Arista-PE32-Q2C-32.00-00       916  48928   745    402 L2  0000.0000.0032.00-00  <>
      Remaining lifetime received: 1195 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Arista-PE32-Q2C-32
      TE IPv4 router ID: 10.0.0.32
      Area addresses: 49.0001
      Topology: 2 (IPv6)
      Topology: 0 (IPv4)
      Interface address: 20.32.175.32
      Interface address: 10.0.0.32
      Interface address: 2001:0:32:175::32
      Interface address: 2002::32
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.32.175.175
        IPv4 Interface Address: 20.32.175.32
        Adj-sid: 362170 flags: [L V] weight: 0x0
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): 1
            TE default metric: 10
            Min/Max unidirectional link delay: 100000/100000 us
      IS Neighbor (MT-IPv6): Juniper-175-ACX7100-48L.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:32:175::175
        Global IPv6 Interface Address: 2001:0:32:175::32
        Adj-sid: 362171 flags: [L V F] weight: 0x0
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): 1
            TE default metric: 10
            Min/Max unidirectional link delay: 100000/100000 us
      Reachability         : 20.32.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 10.0.0.32/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 32 Flags: [N] Algorithm: 0
        SR Prefix-SID: 161 Flags: [N] Algorithm: 128
        SR Prefix-SID: 162 Flags: [N] Algorithm: 129
        SR Prefix-SID: 163 Flags: [N] Algorithm: 130
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
    Arrcus-53.00-00            1434  60822   848    502 L2  0000.0000.0053.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Arrcus-53
      TE IPv4 router ID: 10.0.0.53
      Area addresses: 49.0001
      Topology: 0 (IPv4)
      Topology: 2 (IPv6)
      Interface address: 10.0.0.53
      Interface address: 2002::53
      IS Neighbor          : Ciena-8140-66.00    Metric: 10
        IPv4 Neighbor Address: 20.53.66.66
        IPv4 Interface Address: 20.53.66.53
      IS Neighbor          : Ciena-5134-72.00    Metric: 10
        IPv4 Neighbor Address: 20.53.72.72
        IPv4 Interface Address: 20.53.72.53
      IS Neighbor          : H3C_M1A_120.00      Metric: 10
        IPv4 Neighbor Address: 20.53.120.120
        IPv4 Interface Address: 20.53.120.53
      IS Neighbor          : 0000.0000.0124.00   Metric: 10
        IPv4 Neighbor Address: 20.53.124.124
        IPv4 Interface Address: 20.53.124.53
      IS Neighbor          : 0000.0000.0128.00   Metric: 10
        IPv4 Neighbor Address: 20.53.128.128
        IPv4 Interface Address: 20.53.128.53
      IS Neighbor          : Nokia-IXRe2-216.00  Metric: 10
        IPv4 Neighbor Address: 20.53.216.216
        IPv4 Interface Address: 20.53.216.53
      IS Neighbor          : Keysight-185.00     Metric: 10
        IPv4 Neighbor Address: 20.53.185.185
        IPv4 Interface Address: 20.53.185.53
      IS Neighbor (MT-IPv6): Nokia-IXRe2-216.00  Metric: 10
        IPv4 Interface Address: 20.53.216.53
      Reachability         : 20.53.66.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.53.72.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.53.120.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.53.124.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.53.128.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.53.185.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.53.216.0/24 Metric: 10 Type: 1 Up
      Reachability         : 10.0.0.53/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 53 Flags: [N P E] Algorithm: 0
        SR Prefix-SID: 1181 Flags: [N] Algorithm: 128
        SR Prefix-SID: 1182 Flags: [N] Algorithm: 129
        SR Prefix-SID: 1183 Flags: [N] Algorithm: 130
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
    Arrcus-72XC-2-54.00-00       132  65330   773    165 L2  0000.0000.0054.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Arrcus-72XC-2-54
      TE IPv4 router ID: 10.0.0.54
      Area addresses: 49.0001
      Topology: 0 (IPv4)
      Topology: 2 (IPv6)
      Interface address: 10.0.0.54
      IS Neighbor          : Ciena-8140-66.00    Metric: 10
        IPv4 Neighbor Address: 20.54.66.66
        IPv4 Interface Address: 20.54.66.54
      Reachability         : 20.54.66.0/24 Metric: 10 Type: 1 Up
      Reachability         : 10.0.0.54/32 Metric: 10 Type: 1 Up
        SR Prefix-SID: 54 Flags: [N P E] Algorithm: 0
      Router Capabilities: Router Id: 10.0.0.54 Flags: []
        SR Local Block:
          SRLB Base: 16000 Range: 3001
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 10000
        Algorithms:  0
    Ciena-8140-66.00-00         258  19311   920    809 L2  0000.0000.0066.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4)
      Hostname: Ciena-8140-66
      TE IPv4 router ID: 10.0.0.66
      Area addresses: 65.0001
      Topology: 0 (IPv4)
      Interface address: 10.0.0.66
      IS Neighbor          : Arista-Spine3-Q2A-2-23.00 Metric: 10
        IPv4 Neighbor Address: 20.30.66.30
        IPv4 Interface Address: 20.30.66.66
        Adj-sid: 16014 flags: [L V] weight: 0x0
        Maximum link BW: 10.00 Gbps
        Maximum reservable link BW: 10.00 Gbps
        Unreserved BW:
            TE class 0: 10.00 Gbps	TE class 1: 10.00 Gbps	TE class 2: 10.00 Gbps
            TE class 3: 10.00 Gbps	TE class 4: 10.00 Gbps	TE class 5: 10.00 Gbps
            TE class 6: 10.00 Gbps	TE class 7: 10.00 Gbps
        Local link ID: 1073731833
        Remote link ID: 110
        Application Specific Link Attributes:
          Standard applications: [L] RSVP-TE SR-TE LFA Flex-Algo
      IS Neighbor          : Juniper-179-ACX7024.00 Metric: 10
        IPv4 Neighbor Address: 20.66.179.179
        IPv4 Interface Address: 20.66.179.66
        Adj-sid: 16013 flags: [L V] weight: 0x0
        Maximum link BW: 10.00 Gbps
        Maximum reservable link BW: 10.00 Gbps
        Unreserved BW:
            TE class 0: 10.00 Gbps	TE class 1: 10.00 Gbps	TE class 2: 10.00 Gbps
            TE class 3: 10.00 Gbps	TE class 4: 10.00 Gbps	TE class 5: 10.00 Gbps
            TE class 6: 10.00 Gbps	TE class 7: 10.00 Gbps
        Local link ID: 1073731836
        Remote link ID: 1037
        Application Specific Link Attributes:
          Standard applications: [L] RSVP-TE SR-TE LFA Flex-Algo
      IS Neighbor          : Ericsson_84_R6678.00 Metric: 10
        IPv4 Neighbor Address: 20.66.84.84
        IPv4 Interface Address: 20.66.84.66
        Adj-sid: 16017 flags: [L V] weight: 0x0
        Maximum link BW: 10.00 Gbps
        Maximum reservable link BW: 10.00 Gbps
        Unreserved BW:
            TE class 0: 10.00 Gbps	TE class 1: 10.00 Gbps	TE class 2: 10.00 Gbps
            TE class 3: 10.00 Gbps	TE class 4: 10.00 Gbps	TE class 5: 10.00 Gbps
            TE class 6: 10.00 Gbps	TE class 7: 10.00 Gbps
        Local link ID: 1073731834
        Remote link ID: 83886608
        Application Specific Link Attributes:
          Standard applications: [L] RSVP-TE SR-TE LFA Flex-Algo
      IS Neighbor          : Nokia-SXR-214.00    Metric: 10
        IPv4 Neighbor Address: 20.66.214.214
        IPv4 Interface Address: 20.66.214.66
        Adj-sid: 16015 flags: [L V] weight: 0x0
        Maximum link BW: 10.00 Gbps
        Maximum reservable link BW: 10.00 Gbps
        Unreserved BW:
            TE class 0: 10.00 Gbps	TE class 1: 10.00 Gbps	TE class 2: 10.00 Gbps
            TE class 3: 10.00 Gbps	TE class 4: 10.00 Gbps	TE class 5: 10.00 Gbps
            TE class 6: 10.00 Gbps	TE class 7: 10.00 Gbps
        Local link ID: 1073731838
        Remote link ID: 15
        Application Specific Link Attributes:
          Standard applications: [L] RSVP-TE SR-TE LFA Flex-Algo
      IS Neighbor          : Arrcus-53.00        Metric: 10
        IPv4 Neighbor Address: 20.53.66.53
        IPv4 Interface Address: 20.53.66.66
        Adj-sid: 16016 flags: [L V] weight: 0x0
        Maximum link BW: 10.00 Gbps
        Maximum reservable link BW: 10.00 Gbps
        Unreserved BW:
            TE class 0: 10.00 Gbps	TE class 1: 10.00 Gbps	TE class 2: 10.00 Gbps
            TE class 3: 10.00 Gbps	TE class 4: 10.00 Gbps	TE class 5: 10.00 Gbps
            TE class 6: 10.00 Gbps	TE class 7: 10.00 Gbps
        Local link ID: 1073731837
        Remote link ID: 1021
        Application Specific Link Attributes:
          Standard applications: [L] RSVP-TE SR-TE LFA Flex-Algo
      IS Neighbor          : Arrcus-72XC-2-54.00 Metric: 10
        IPv4 Neighbor Address: 20.54.66.54
        IPv4 Interface Address: 20.54.66.66
        Adj-sid: 16018 flags: [L V] weight: 0x0
        Maximum link BW: 10.00 Gbps
        Maximum reservable link BW: 10.00 Gbps
        Unreserved BW:
            TE class 0: 10.00 Gbps	TE class 1: 10.00 Gbps	TE class 2: 10.00 Gbps
            TE class 3: 10.00 Gbps	TE class 4: 10.00 Gbps	TE class 5: 10.00 Gbps
            TE class 6: 10.00 Gbps	TE class 7: 10.00 Gbps
        Local link ID: 1073731835
        Remote link ID: 1008
        Application Specific Link Attributes:
          Standard applications: [L] RSVP-TE SR-TE LFA Flex-Algo
      IS Neighbor          : Juniper-156-PTX10002-36QDD.00 Metric: 10
        IPv4 Neighbor Address: 20.66.156.156
        IPv4 Interface Address: 20.66.156.66
        Adj-sid: 16019 flags: [L V] weight: 0x0
        Maximum link BW: 100.00 Gbps
        Maximum reservable link BW: 100.00 Gbps
        Unreserved BW:
            TE class 0: 100.00 Gbps	TE class 1: 100.00 Gbps	TE class 2: 100.00 Gbps
            TE class 3: 100.00 Gbps	TE class 4: 100.00 Gbps	TE class 5: 100.00 Gbps
            TE class 6: 100.00 Gbps	TE class 7: 100.00 Gbps
        Local link ID: 1073731840
        Remote link ID: 1049
        Application Specific Link Attributes:
          Standard applications: [L] RSVP-TE SR-TE LFA Flex-Algo
      Reachability         : 10.0.0.66/32 Metric: 10 Type: 1 Up
        SR Prefix-SID: 66 Flags: [N] Algorithm: 0
      Reachability         : 20.30.66.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.66.84.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.54.66.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.66.179.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.53.66.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.66.214.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.66.156.0/24 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.66 Flags: []
        SR Capability: Flags: [I]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0
    Ciena-5134-72.00-00          82  49033   974    209 L2  0000.0000.0072.00-00  <>
      Remaining lifetime received: 1198 s Modified to: 1200 s
      NLPID: 0xCC(IPv4)
      Hostname: Ciena-5134-72
      TE IPv4 router ID: 10.0.0.72
      Area addresses: 65.0001
      Topology: 0 (IPv4)
      Interface address: 10.0.0.72
      IS Neighbor          : Arrcus-53.00        Metric: 10
        IPv4 Neighbor Address: 20.53.72.53
        IPv4 Interface Address: 20.53.72.72
        Adj-sid: 16004 flags: [L V] weight: 0x0
        Maximum link BW: 10.00 Gbps
        Maximum reservable link BW: 10.00 Gbps
        Unreserved BW:
            TE class 0: 10.00 Gbps	TE class 1: 10.00 Gbps	TE class 2: 10.00 Gbps
            TE class 3: 10.00 Gbps	TE class 4: 10.00 Gbps	TE class 5: 10.00 Gbps
            TE class 6: 10.00 Gbps	TE class 7: 10.00 Gbps
        Local link ID: 1073731835
        Remote link ID: 1022
        Application Specific Link Attributes:
          Standard applications: [L] RSVP-TE SR-TE LFA Flex-Algo
      Reachability         : 20.53.72.0/24 Metric: 10 Type: 1 Up
      Reachability         : 10.0.0.72/32 Metric: 10 Type: 1 Up
        SR Prefix-SID: 72 Flags: [N] Algorithm: 0
      Router Capabilities: Router Id: 10.0.0.72 Flags: []
        SR Capability: Flags: [I]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0
    Ericsson_84_R6678.00-00        89  34909   943    187 L2  0000.0000.0084.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Ericsson_84_R6678
      TE IPv4 router ID: 10.0.0.84
      Area addresses: 65.0000
      Topology: 0 (IPv4)
      Topology: 2 (IPv6)
      Interface address: 10.0.0.84
      Interface address: 2001:0:66:84::84
      IS Neighbor          : Ciena-8140-66.00    Metric: 10
        IPv4 Interface Address: 20.66.84.84
      Reachability         : 10.0.0.84/32 Metric: 10 Type: 1 Up
        SR Prefix-SID: 84 Flags: [N P] Algorithm: 0
      Reachability (MT-IPv6): 2001:0:66:84::/64 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.84 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  8
        SR Capability: Flags: [I]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0
    H3C_M1A_120.00-00         13915  22798  1193   1239 L2  0000.0000.0120.00-00  <>
      Remaining lifetime received: 13 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: H3C_M1A_120
      TE IPv4 router ID: 10.0.0.120
      Area addresses: 49.0001
      Topology: 0 (IPv4)
      Topology: 2 (IPv6)
      Interface address: 10.0.0.120
      Interface address: 20.53.120.120
      Interface address: 20.120.175.120
      Interface address: 20.120.214.120
      Interface address: 21.120.175.120
      Interface address: 2001:0:120:214::120
      Interface address: 2002::120
      IS Neighbor          : Arrcus-53.00        Metric: 2
        IPv4 Neighbor Address: 20.53.120.53
        IPv4 Interface Address: 20.53.120.120
        Adj-sid: 1147 flags: [L V] weight: 0x0
        TE default metric: 2
        Maximum link BW: 0.00 bps
        Maximum reservable link BW: 0.00 bps
        Unreserved BW:
            TE class 0: 0.00 bps	TE class 1: 0.00 bps	TE class 2: 0.00 bps
            TE class 3: 0.00 bps	TE class 4: 0.00 bps	TE class 5: 0.00 bps
            TE class 6: 0.00 bps	TE class 7: 0.00 bps
        Local link ID: 7
        Remote link ID: 1009
      IS Neighbor          : Arrcus-53.00        Metric: 2
        IPv4 Neighbor Address: 20.53.120.53
        IPv4 Interface Address: 20.53.120.120
        Local link ID: 7
        Remote link ID: 1009
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
          User-defined applications: APP3
            TE default metric: 2
            Maximum link BW: 0.00 bps
            Maximum reservable link BW: 0.00 bps
            Unreserved BW:
                TE class 0: 0.00 bps	TE class 1: 0.00 bps	TE class 2: 0.00 bps
                TE class 3: 0.00 bps	TE class 4: 0.00 bps	TE class 5: 0.00 bps
                TE class 6: 0.00 bps	TE class 7: 0.00 bps
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 1
        IPv4 Neighbor Address: 20.120.175.175
        IPv4 Interface Address: 20.120.175.120
        Adj-sid: 1151 flags: [L V] weight: 0x0
        TE default metric: 1
        Maximum link BW: 0.00 bps
        Maximum reservable link BW: 0.00 bps
        Unreserved BW:
            TE class 0: 0.00 bps	TE class 1: 0.00 bps	TE class 2: 0.00 bps
            TE class 3: 0.00 bps	TE class 4: 0.00 bps	TE class 5: 0.00 bps
            TE class 6: 0.00 bps	TE class 7: 0.00 bps
        Local link ID: 4
        Remote link ID: 1007
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 1
        IPv4 Neighbor Address: 20.120.175.175
        IPv4 Interface Address: 20.120.175.120
        Local link ID: 4
        Remote link ID: 1007
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
          User-defined applications: APP3
            TE default metric: 1
            Maximum link BW: 0.00 bps
            Maximum reservable link BW: 0.00 bps
            Unreserved BW:
                TE class 0: 0.00 bps	TE class 1: 0.00 bps	TE class 2: 0.00 bps
                TE class 3: 0.00 bps	TE class 4: 0.00 bps	TE class 5: 0.00 bps
                TE class 6: 0.00 bps	TE class 7: 0.00 bps
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 2
        IPv4 Neighbor Address: 21.120.175.175
        IPv4 Interface Address: 21.120.175.120
        Adj-sid: 1148 flags: [L V] weight: 0x0
        TE default metric: 2
        Maximum link BW: 0.00 bps
        Maximum reservable link BW: 0.00 bps
        Unreserved BW:
            TE class 0: 0.00 bps	TE class 1: 0.00 bps	TE class 2: 0.00 bps
            TE class 3: 0.00 bps	TE class 4: 0.00 bps	TE class 5: 0.00 bps
            TE class 6: 0.00 bps	TE class 7: 0.00 bps
        Local link ID: 6
        Remote link ID: 1058
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 2
        IPv4 Neighbor Address: 21.120.175.175
        IPv4 Interface Address: 21.120.175.120
        Local link ID: 6
        Remote link ID: 1058
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
          User-defined applications: APP3
            TE default metric: 2
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
      Reachability         : 20.53.120.0/24 Metric: 2 Type: 1 Up
      Reachability         : 20.120.175.0/24 Metric: 1 Type: 1 Up
      Reachability         : 20.120.214.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.120.217.0/24 Metric: 0 Type: 1 Up
      Reachability         : 21.120.175.0/24 Metric: 2 Type: 1 Up
      Reachability         : 192.168.20.0/23 Metric: 0 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:53:120::/64 Metric: 0 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:120:175::/64 Metric: 0 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:120:214::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:120:217::/64 Metric: 0 Type: 1 Up
      Reachability (MT-IPv6): 2001:1:120:175::/64 Metric: 0 Type: 1 Up
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
      Shared Risk Link Group:  Neighbor Juniper-175-ACX7100-48L.00 (Numbered)
        Interface Address: 20.120.175.120
        Neighbor Address: 20.120.175.175
        Group ID: 4
      Application Specific Shared Risk Link Group:  Neighbor Juniper-175-ACX7100-48L.00
        Standard applications: Flex-Algo
        User-defined applications: APP3
        Local link identifier: 343453560
        Remote link identifier: 343453615
        IPv4 interface address: 20.120.175.120
        IPv4 neighbor address: 20.120.175.175
        Group ID: 4
    0000.0000.0124.00-00       2067   4938  1177    151 L2  0000.0000.0124.00-00  <>
      Remaining lifetime received: 1198 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      TE IPv4 router ID: 10.0.0.124
      Area addresses: 49.0001
      Topology: 0 (IPv4)
      Topology: 2 (IPv6)
      Interface address: 10.0.0.124
      Interface address: 20.53.124.124
      IS Neighbor          : Arrcus-53.00        Metric: 10
        IPv4 Neighbor Address: 20.53.124.53
        IPv4 Interface Address: 20.53.124.124
        Adj-sid: 272 flags: [L V] weight: 0x0
        Local link ID: 9
        Remote link ID: 1025
      Reachability         : 10.0.0.124/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 124 Flags: [N P] Algorithm: 0
      Reachability         : 20.53.124.0/24 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.124 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  10
        SR Capability: Flags: [I]
          SRGB Base: 2000 Range: 2001
    0000.0000.0128.00-00       2072  10071   935    151 L2  0000.0000.0128.00-00  <>
      Remaining lifetime received: 1198 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      TE IPv4 router ID: 10.0.0.128
      Area addresses: 49.0001
      Topology: 0 (IPv4)
      Topology: 2 (IPv6)
      Interface address: 10.0.0.128
      Interface address: 20.53.128.128
      IS Neighbor          : Arrcus-53.00        Metric: 10
        IPv4 Neighbor Address: 20.53.128.53
        IPv4 Interface Address: 20.53.128.128
        Adj-sid: 48000 flags: [L V] weight: 0x0
        Local link ID: 14
        Remote link ID: 1029
      Reachability         : 10.0.0.128/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 128 Flags: [N] Algorithm: 0
      Reachability         : 20.53.128.0/24 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.128 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  10
        SR Capability: Flags: [I]
          SRGB Base: 20000 Range: 2000
    Juniper-131-JCNR.00-00       674  45598   631    338 L2  0000.0000.0131.00-00  <>
      Remaining lifetime received: 1194 s Modified to: 1200 s
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
      Reachability         : 20.131.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 10.0.0.131/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 131 Flags: [N] Algorithm: 0
      Reachability          : 2001:0:131:175::/64 Metric: 10 Type: 1 Up
      Reachability          : fe80::ec97:fbff:fe06:5964/128 Metric: 0 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.131 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  0
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0, 1, 128, 129, 130
      Unsupported TLV: Type: 14 Length: 2
    Juniper-175-ACX7100-48L.00-00      1232  12825   510   1280 L2  0000.0000.0175.00-00  <>
      Remaining lifetime received: 1196 s Modified to: 1200 s
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
      IS Neighbor          : Juniper-179-ACX7024.00 Metric: 1
        IPv4 Neighbor Address: 21.175.179.179
        IPv4 Interface Address: 21.175.179.175
        IPv6 Neighbor Address: 2001:1:175::179:179
        Global IPv6 Interface Address: 2001:1:175::179:175
        Adj-sid: 177 flags: [L V B] weight: 0x0
        TE default metric: 10
        Min/Max unidirectional link delay: 100000/100000 us
        Average unidirectional link delay: 100000 us
        Local link ID: 1046
        Remote link ID: 1032
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
        Adj-sid: 197 flags: [L V] weight: 0x0
        TE default metric: 10
        Min/Max unidirectional link delay: 100000/100000 us
        Average unidirectional link delay: 100000 us
        Local link ID: 1003
        Remote link ID: 7
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): 1
            TE default metric: 10
            Min/Max unidirectional link delay: 100000/100000 us
      IS Neighbor          : 221.00              Metric: 10
        IPv4 Neighbor Address: 20.175.221.221
        IPv4 Interface Address: 20.175.221.175
        Global IPv6 Interface Address: 2001:0:175:221::175
        Adj-sid: 199 flags: [L V] weight: 0x0
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
      IS Neighbor (MT-IPv6): Nokia-SR1-217.00    Metric: 10
        IPv4 Interface Address: 20.175.217.175
        IPv6 Neighbor Address: 2001:0:175:217::217
        Global IPv6 Interface Address: 2001:0:175:217::175
        Adj-sid: 198 flags: [L V F] weight: 0x0
        TE default metric: 10
        Min/Max unidirectional link delay: 100000/100000 us
        Average unidirectional link delay: 100000 us
        Local link ID: 1003
        Remote link ID: 7
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
      Reachability         : 20.66.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.72.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.175.214.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.131.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.32.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 21.175.179.0/24 Metric: 1 Type: 1 Up
      Reachability         : 20.175.179.0/24 Metric: 1 Type: 1 Up
      Reachability         : 20.175.184.0/24 Metric: 10 Type: 1 Up
      Reachability         : 21.120.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.120.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.175.217.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.128.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.175.221.0/24 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2002::175/128 Metric: 0 Type: 1 Up
        SR Prefix-SID: 575 Flags: [N] Algorithm: 0
        SR Prefix-SID: 1705 Flags: [N] Algorithm: 130
        SR Prefix-SID: 1704 Flags: [N] Algorithm: 129
        SR Prefix-SID: 1703 Flags: [N] Algorithm: 128
      Reachability (MT-IPv6): 2001:0:175:214::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:66:175::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:72:175::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:32:175::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:1:175::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:175::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:175:184::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:120:175::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:1:120:175::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:175:217::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:128:175::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:175:221::/64 Metric: 10 Type: 1 Up
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
      Shared Risk Link Group:  Neighbor Juniper-179-ACX7024.00 (Numbered)
        Interface Address: 21.175.179.175
        Neighbor Address: 21.175.179.179
        Group ID: 4
      Unsupported TLV: Type: 14 Length: 2
    Juniper-175-ACX7100-48L.00-01       995   2531   715    299 L2  0000.0000.0175.00-01  <>
      Remaining lifetime received: 1196 s Modified to: 1200 s
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
    Juniper-175-ACX7100-48L.00-02       675   4392   873    434 L2  0000.0000.0175.00-02  <>
      Remaining lifetime received: 1196 s Modified to: 1200 s
      IS Neighbor          : Juniper-179-ACX7024.00 Metric: 1
        IPv4 Neighbor Address: 20.175.179.179
        IPv4 Interface Address: 20.175.179.175
        IPv6 Neighbor Address: 2001:0:175::179:179
        Global IPv6 Interface Address: 2001:0:175::179:175
        Adj-sid: 187 flags: [L V B] weight: 0x0
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
        IPv4 Neighbor Address: 21.120.175.120
        IPv4 Interface Address: 21.120.175.175
        Global IPv6 Interface Address: 2001:1:120:175::175
        Adj-sid: 195 flags: [L V] weight: 0x0
        TE default metric: 10
        Min/Max unidirectional link delay: 100000/100000 us
        Average unidirectional link delay: 100000 us
        Local link ID: 1058
        Remote link ID: 6
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): 1
            TE default metric: 10
            Min/Max unidirectional link delay: 100000/100000 us
      IS Neighbor          : H3C_M1A_120.00      Metric: 10
        IPv4 Neighbor Address: 20.120.175.120
        IPv4 Interface Address: 20.120.175.175
        Global IPv6 Interface Address: 2001:0:120:175::175
        Adj-sid: 194 flags: [L V] weight: 0x0
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
      Shared Risk Link Group:  Neighbor Juniper-179-ACX7024.00 (Numbered)
        Interface Address: 20.175.179.175
        Neighbor Address: 20.175.179.179
        Group ID: 4
 H  Juniper-179-ACX7024.00-00       879   3953  1006    464 L2  0000.0000.0179.00-00  <>
      Remaining lifetime received: 1194 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Juniper-179-ACX7024
      TE IPv4 router ID: 10.0.0.179
      TE IPv6 router ID: 2001:0:175::179:179
      Area addresses: 49.0001
      Interface address: 10.0.0.179
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.175.179.175
        IPv4 Interface Address: 20.175.179.179
        IPv6 Neighbor Address: 2001:0:175::179:175
        Global IPv6 Interface Address: 2001:0:175::179:179
        Adj-sid: 29 flags: [L V F] weight: 0x0
        Adj-sid: 28 flags: [L V] weight: 0x0
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
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 21.175.179.175
        IPv4 Interface Address: 21.175.179.179
        IPv6 Neighbor Address: 2001:1:175::179:175
        Global IPv6 Interface Address: 2001:1:175::179:179
        Adj-sid: 26 flags: [L V F] weight: 0x0
        Adj-sid: 25 flags: [L V] weight: 0x0
        TE default metric: 10
        Min/Max unidirectional link delay: 100000/100000 us
        Average unidirectional link delay: 100000 us
        Local link ID: 1032
        Remote link ID: 1046
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): 1
            Min/Max unidirectional link delay: 100000/100000 us
      Reachability         : 10.0.0.179/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 179 Flags: [N] Algorithm: 0
        SR Prefix-SID: 1307 Flags: [N] Algorithm: 128
        SR Prefix-SID: 1308 Flags: [N] Algorithm: 129
        SR Prefix-SID: 1309 Flags: [N] Algorithm: 130
      Router Capabilities: Router Id: 10.0.0.179 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  8
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0, 1, 128, 129, 130
      Unsupported TLV: Type: 14 Length: 2
    Nokia-SXR-214.00-00       24159  55016  1199    257 L2  0000.0000.0214.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Nokia-SXR-214
      TE IPv4 router ID: 10.0.0.214
      TE IPv6 router ID: 2000::214
      Area addresses: 49.0001
      Topology: 0 (IPv4)
      Topology: 2 (IPv6)
      Interface address: 10.0.0.214
      Interface address: 20.66.214.214
      Interface address: 2000::214
      Interface address: 2001:0:66:214::214
      IS Neighbor          : Ciena-8140-66.00    Metric: 10
        IPv4 Neighbor Address: 20.66.214.66
        IPv4 Interface Address: 20.66.214.214
        Adj-sid: 30045 flags: [L V B] weight: 0x0
      Reachability         : 20.66.214.0/24 Metric: 10 Type: 1 Up
      Reachability         : 10.0.0.214/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 214 Flags: [N P] Algorithm: 0
      Reachability (MT-IPv6): 2000::214/128 Metric: 0 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:66:214::/64 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.214 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  15
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0
    Arista-Spine3-Q2A-2-23.00-00        92  26037   635    167 L2  0000.0000.3030.00-00  <>
      LSP generation remaining wait time: 0 ms
      Time remaining until refresh: 335 s
      NLPID: 0xCC(IPv4)
      Hostname: Arista-Spine3-Q2A-2-23
      Area addresses: 49.0001
      Interface address: 10.0.30.30
      Interface address: 20.30.66.30
      IS Neighbor          : Ciena-8140-66.00    Metric: 1
        IPv4 Neighbor Address: 20.30.66.66
        IPv4 Interface Address: 20.30.66.30
        Adj-sid: 378674 flags: [L V] weight: 0x0
      Reachability         : 10.0.30.30/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 330 Flags: [N] Algorithm: 0
      Reachability         : 20.30.66.0/24 Metric: 1 Type: 1 Up
      Router Capabilities: Router Id: 10.0.30.30 Flags: []
        SR Local Block:
          SRLB Base: 965536 Range: 65536
        Area leader priority: 250 algorithm: 0
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  12
        SR Capability: Flags: [I]
          SRGB Base: 20000 Range: 2000
    Juniper-156-PTX10002-36QDD.00-00       107  49284   814    291 L2  0000.0001.0156.00-00  <>
      Remaining lifetime received: 1198 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Juniper-156-PTX10002-36QDD
      TE IPv4 router ID: 10.0.0.156
      TE IPv6 router ID: 2002::156
      Area addresses: 49.0001
      Interface address: 10.0.0.156
      Interface address: 10.0.1.156
      Interface address: 2002::156
      IS Neighbor          : Nokia-IXRe2-216.00  Metric: 10
        IPv4 Neighbor Address: 20.156.216.216
        IPv4 Interface Address: 20.156.216.156
        Adj-sid: 28 flags: [L V] weight: 0x0
        Maximum link BW: 100.00 Gbps
        Local link ID: 1038
        Remote link ID: 24
      IS Neighbor          : Ciena-8140-66.00    Metric: 10
        IPv4 Neighbor Address: 20.66.156.66
        IPv4 Interface Address: 20.66.156.156
        Adj-sid: 29 flags: [L V] weight: 0x0
        Maximum link BW: 100.00 Gbps
        Local link ID: 1049
        Remote link ID: 1073731840
      Reachability         : 10.0.1.156/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 456 Flags: [N] Algorithm: 0
      Router Capabilities: Router Id: 10.0.0.156 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  0
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0, 1
      Unsupported TLV: Type: 14 Length: 2
 H  Juniper-179-ACX7024.00-00       567  25367   952    222 L2  0000.0001.0179.00-00  <>
      Remaining lifetime received: 1198 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Juniper-179-ACX7024
      TE IPv4 router ID: 10.0.0.179
      TE IPv6 router ID: 2001:0:175::179:179
      Area addresses: 49.0001
      Interface address: 10.0.0.179
      Interface address: 10.0.1.179
      IS Neighbor          : Ciena-8140-66.00    Metric: 10
        IPv4 Neighbor Address: 20.66.179.66
        IPv4 Interface Address: 20.66.179.179
        Adj-sid: 31 flags: [L V] weight: 0x0
        Maximum link BW: 10.00 Gbps
        Local link ID: 1037
        Remote link ID: 1073731836
      Reachability         : 10.0.1.179/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 479 Flags: [N] Algorithm: 0
      Router Capabilities: Router Id: 10.0.0.179 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  8
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0, 1
      Unsupported TLV: Type: 14 Length: 2
    Nokia-IXRe2-216.00-00      1848  43736  1110    322 L2  0100.0000.0216.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Nokia-IXRe2-216
      TE IPv4 router ID: 10.0.0.216
      TE IPv6 router ID: 2002::216
      Area addresses: 49.0001.0000.0000.0216.00
      Topology: 0 (IPv4)
      Topology: 2 (IPv6)
      Interface address: 10.0.0.216
      Interface address: 20.53.216.216
      Interface address: 20.156.216.216
      Interface address: 2001:0:53:216::216
      Interface address: 2002::216
      IS Neighbor          : Arrcus-53.00        Metric: 10
        IPv4 Neighbor Address: 20.53.216.53
        IPv4 Interface Address: 20.53.216.216
        Adj-sid: 1048574 flags: [L V B] weight: 0x0
      IS Neighbor          : Juniper-156-PTX10002-36QDD.00 Metric: 10
        IPv4 Neighbor Address: 20.156.216.156
        IPv4 Interface Address: 20.156.216.216
        Adj-sid: 1048572 flags: [L V B] weight: 0x0
      IS Neighbor (MT-IPv6): Arrcus-53.00        Metric: 10
      Reachability         : 20.53.216.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.156.216.0/24 Metric: 10 Type: 1 Up
      Reachability         : 10.0.0.216/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 216 Flags: [N P] Algorithm: 0
      Reachability (MT-IPv6): 2001:0:53:216::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2002::216/128 Metric: 0 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.216 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  11
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0
    Nokia-SR1-217.00-00        1285  45905   621    392 L2  0100.0000.0217.00-00  <>
      Remaining lifetime received: 1196 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Nokia-SR1-217
      TE IPv4 router ID: 10.0.0.217
      TE IPv6 router ID: 2002::217
      Area addresses: 49.0001.0000.0000.0217.00
      Topology: 0 (IPv4)
      Topology: 2 (IPv6)
      Interface address: 10.0.0.217
      Interface address: 20.175.217.217
      Interface address: 2001:0:175:217::217
      Interface address: 2002::217
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.175.217.175
        IPv4 Interface Address: 20.175.217.217
        Adj-sid: 524268 flags: [L V B] weight: 0x0
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
      IS Neighbor (MT-IPv6): Juniper-175-ACX7100-48L.00 Metric: 10
      Reachability         : 10.0.0.217/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 57 Flags: [N P] Algorithm: 0
        SR Prefix-SID: 1345 Flags: [N P] Algorithm: 128
        SR Prefix-SID: 1346 Flags: [N P] Algorithm: 129
        SR Prefix-SID: 1347 Flags: [N P] Algorithm: 130
      Reachability         : 20.175.217.0/24 Metric: 10 Type: 1 Up
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
    221.00-00                   860  59290  1118     86 L2  0221.0221.0221.00-00  <>
      Remaining lifetime received: 1196 s Modified to: 1200 s
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
        Algorithms:  0, 128, 129, 130
      Unsupported TLV: Type: 14 Length: 2
    221.00-01                    90  11242  1194     32 L2  0221.0221.0221.00-01  <>
      Remaining lifetime received: 1196 s Modified to: 1200 s
      Hostname: 221
    221.00-02                   607  14667  1003    305 L2  0221.0221.0221.00-02  <>
      Remaining lifetime received: 1196 s Modified to: 1200 s
      Interface address: 10.0.0.221
      Interface address: 20.175.221.221
      Interface address: 1221::1
      Interface address: 2001:0:175:221::221
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.175.221.175
        IPv4 Interface Address: 20.175.221.221
        Adj-sid: 524293 flags: [L V B] weight: 0x0
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
      Reachability         : 10.0.0.221/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 221 Flags: [N] Algorithm: 0
        SR Prefix-SID: 1349 Flags: [N] Algorithm: 128
        SR Prefix-SID: 1350 Flags: [N] Algorithm: 129
        SR Prefix-SID: 1351 Flags: [N] Algorithm: 130
      Reachability         : 20.175.221.0/24 Metric: 10 Type: 1 Up
      Reachability          : 1221::1/128 Metric: 0 Type: 1 Up
      Reachability          : 2001:0:175:221::/64 Metric: 10 Type: 1 Up
    Keysight-185.00-00            8   8805   753    132 L2  6500.0000.0185.00-00  <DefaultAtt>
      Remaining lifetime received: 1195 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6) 0x81(CLNP)
      Hostname: Keysight-185
      Area addresses: 49.0001
      Interface address: 20.53.185.185
      IS Neighbor          : Arrcus-53.00        Metric: 10
        Adj-sid: 9001 flags: [L V] weight: 0x0
      Reachability         : 10.0.0.185/32 Metric: 10 Type: 1 Up
        SR Prefix-SID: 185 Flags: [N] Algorithm: 0
      Reachability         : 20.53.185.0/24 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.185 Flags: []
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0

Legend:
H - hostname conflict
U - node unreachable

IS-IS Instance: IGP VRF: default
  IS-IS Level 2 Link State Database
    LSPID                   Seq Num  Cksum  Life Length IS  Received LSPID        Flags
    Arista-Spine3-Q2A-30.00-00      6990  51392   738    313 L2  0000.0000.0030.00-00  <>
      LSP generation remaining wait time: 0 ms
      Time remaining until refresh: 438 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Arista-Spine3-Q2A-30
      TE IPv4 router ID: 10.0.0.30
      Area addresses: 49.0001
      Topology: 2 (IPv6)
      Topology: 0 (IPv4)
      Interface address: 10.0.0.30
      Interface address: 20.30.184.30
      Interface address: 2002::30
      Interface address: 2001:0:30:184::30
      Reachability         : 10.0.0.30/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 30 Flags: [N] Algorithm: 0
        SR Prefix-SID: 158 Flags: [N] Algorithm: 128
        SR Prefix-SID: 159 Flags: [N] Algorithm: 129
        SR Prefix-SID: 160 Flags: [N] Algorithm: 130
      Reachability         : 20.30.184.0/24 Metric: 1 Type: 1 Up
      Reachability (MT-IPv6): 2002::30/128 Metric: 10 Type: 1 Up
        SR Prefix-SID: 430 Flags: [N] Algorithm: 0
        SR Prefix-SID: 558 Flags: [N] Algorithm: 128
        SR Prefix-SID: 559 Flags: [N] Algorithm: 129
        SR Prefix-SID: 560 Flags: [N] Algorithm: 130
      Reachability (MT-IPv6): 2001:0:30:184::/64 Metric: 10 Type: 1 Up
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
Last updated: 19:46:34 ago
Next Hop Interface
-------- ---------

Destination: Arista-Spine3-Q2A-30
Path ID: 641
Path constraints: algo MIN-TE
                  metric type TE
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 1
Last updated: 19:46:34 ago
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
Last updated: 19:46:34 ago
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
Last updated: 19:46:34 ago
Next Hop Interface
-------- ---------

Destination: Arista-Spine3-Q2A-30
Path ID: 641
Path constraints: algo MIN-TE
                  metric type TE
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 1
Last updated: 19:46:34 ago
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
Last updated: 19:46:34 ago
Next Hop Interface
-------- ---------

```

## show isis segment-routing tunnel

```text
  Index     Endpoint          Next Hop/Tunnel Index     Interface     Labels   
--------- ----------------- ------------------------- --------------- ---------
  7         10.0.0.175/32     20.30.66.66               Ethernet31    [ 20175 ]
  8         10.0.0.84/32      20.30.66.66               Ethernet31    [ 20084 ]
  9         10.0.0.131/32     20.30.66.66               Ethernet31    [ 20131 ]
  10        10.0.0.53/32      20.30.66.66               Ethernet31    [ 20053 ]
  12        10.0.0.179/32     20.30.66.66               Ethernet31    [ 20179 ]
  13        10.0.0.66/32      20.30.66.66               Ethernet31    [ 3 ]    
  14        10.0.0.72/32      20.30.66.66               Ethernet31    [ 20072 ]
  15        10.0.0.221/32     20.30.66.66               Ethernet31    [ 20221 ]
  16        10.0.0.217/32     20.30.66.66               Ethernet31    [ 20057 ]
  17        10.0.0.120/32     20.30.66.66               Ethernet31    [ 20120 ]
  18        10.0.0.128/32     20.30.66.66               Ethernet31    [ 20128 ]
  20        10.0.0.32/32      20.30.66.66               Ethernet31    [ 20032 ]
  21        10.0.0.214/32     20.30.66.66               Ethernet31    [ 20214 ]
  22        10.0.0.124/32     20.30.66.66               Ethernet31    [ 20124 ]
  23        10.0.1.179/32     20.30.66.66               Ethernet31    [ 20479 ]
  24        10.0.1.156/32     20.30.66.66               Ethernet31    [ 20456 ]
  25        10.0.0.216/32     20.30.66.66               Ethernet31    [ 20216 ]
  28        10.0.0.185/32     20.30.66.66               Ethernet31    [ 20185 ]
  29        10.0.0.54/32      20.30.66.66               Ethernet31    [ 20054 ]

```

## show isis segment-routing prefix-segments

```text

System ID: Arista-Spine3-Q2A-2-23			Instance: '2-23-5G'
SR supported Data-plane: MPLS			SR Router ID: 10.0.30.30

Node: 41     Proxy-Node: 0      Prefix: 0       Total Segments: 41

Flag Descriptions: R: Re-advertised, N: Node Segment, P: no-PHP
                   E: Explicit-NULL, V: Value, L: Local
Segment status codes: * - Self originated Prefix, L1 - level 1, L2 - level 2, ! - SR-unreachable,
                      # - Some IS-IS next-hops are SR-unreachable
   Prefix                      SID   Label Type       Flags                        System ID       Level Protection  Algorithm   
   ------------------------- ----- ------- ---------- ---------------------------- --------------- ----- ----------- -------------
   10.0.0.32/32                 32   20032 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-PE32-Q2C-32 L2    unprotected SPF         
   10.0.0.32/32                161   20161 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-PE32-Q2C-32 L2    unprotected MIN-LATENCY 
   10.0.0.32/32                162   20162 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-PE32-Q2C-32 L2    unprotected MIN-TE      
   10.0.0.32/32                163   20163 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-PE32-Q2C-32 L2    unprotected ADMIN       
   10.0.0.53/32                 53   20053 Node       R:0 N:1 P:1 E:1 V:0 L:0      Arrcus-53       L2    unprotected SPF         
   10.0.0.53/32               1181   21181 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arrcus-53       L2    unprotected MIN-LATENCY 
   10.0.0.53/32               1182   21182 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arrcus-53       L2    unprotected MIN-TE      
   10.0.0.53/32               1183   21183 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arrcus-53       L2    unprotected ADMIN       
   10.0.0.54/32                 54   20054 Node       R:0 N:1 P:1 E:1 V:0 L:0      Arrcus-72XC-2-54 L2    unprotected SPF         
   10.0.0.66/32                 66   20066 Node       R:0 N:1 P:0 E:0 V:0 L:0      Ciena-8140-66   L2    unprotected SPF         
   10.0.0.72/32                 72   20072 Node       R:0 N:1 P:0 E:0 V:0 L:0      Ciena-5134-72   L2    unprotected SPF         
   10.0.0.84/32                 84   20084 Node       R:0 N:1 P:1 E:0 V:0 L:0      Ericsson_84_R6678 L2    unprotected SPF         
   10.0.0.120/32               120   20120 Node       R:0 N:1 P:0 E:0 V:0 L:0      H3C_M1A_120     L2    unprotected SPF         
   10.0.0.120/32              1248   21248 Node       R:0 N:1 P:0 E:0 V:0 L:0      H3C_M1A_120     L2    unprotected MIN-LATENCY 
   10.0.0.120/32              1249   21249 Node       R:0 N:1 P:0 E:0 V:0 L:0      H3C_M1A_120     L2    unprotected MIN-TE      
   10.0.0.120/32              1250   21250 Node       R:0 N:1 P:0 E:0 V:0 L:0      H3C_M1A_120     L2    unprotected ADMIN       
   10.0.0.124/32               124    2124 Node       R:0 N:1 P:1 E:0 V:0 L:0      0000.0000.0124  L2    unprotected SPF         
   10.0.0.128/32               128   20128 Node       R:0 N:1 P:0 E:0 V:0 L:0      0000.0000.0128  L2    unprotected SPF         
   10.0.0.131/32               131   20131 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-131-JCNR L2    unprotected SPF         
   10.0.0.175/32               175   20175 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-175-ACX7100-48L L2    unprotected SPF         
   10.0.0.175/32              1303   21303 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-175-ACX7100-48L L2    unprotected MIN-LATENCY 
   10.0.0.175/32              1304   21304 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-175-ACX7100-48L L2    unprotected MIN-TE      
   10.0.0.175/32              1305   21305 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-175-ACX7100-48L L2    unprotected ADMIN       
   10.0.0.179/32               179   20179 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-179-ACX7024 L2    unprotected SPF         
   10.0.0.179/32              1307   21307 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-179-ACX7024 L2    unprotected MIN-LATENCY 
   10.0.0.179/32              1308   21308 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-179-ACX7024 L2    unprotected MIN-TE      
   10.0.0.179/32              1309   21309 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-179-ACX7024 L2    unprotected ADMIN       
   10.0.0.185/32               185   20185 Node       R:0 N:1 P:0 E:0 V:0 L:0      Keysight-185    L2    unprotected SPF         
   10.0.0.214/32               214   20214 Node       R:0 N:1 P:1 E:0 V:0 L:0      Nokia-SXR-214   L2    unprotected SPF         
   10.0.0.216/32               216   20216 Node       R:0 N:1 P:1 E:0 V:0 L:0      Nokia-IXRe2-216 L2    unprotected SPF         
   10.0.0.217/32                57   20057 Node       R:0 N:1 P:1 E:0 V:0 L:0      Nokia-SR1-217   L2    unprotected SPF         
   10.0.0.217/32              1345   21345 Node       R:0 N:1 P:1 E:0 V:0 L:0      Nokia-SR1-217   L2    unprotected MIN-LATENCY 
   10.0.0.217/32              1346   21346 Node       R:0 N:1 P:1 E:0 V:0 L:0      Nokia-SR1-217   L2    unprotected MIN-TE      
   10.0.0.217/32              1347   21347 Node       R:0 N:1 P:1 E:0 V:0 L:0      Nokia-SR1-217   L2    unprotected ADMIN       
   10.0.0.221/32               221  720221 Node       R:0 N:1 P:0 E:0 V:0 L:0      221             L2    unprotected SPF         
   10.0.0.221/32              1349  721349 Node       R:0 N:1 P:0 E:0 V:0 L:0      221             L2    unprotected MIN-LATENCY 
   10.0.0.221/32              1350  721350 Node       R:0 N:1 P:0 E:0 V:0 L:0      221             L2    unprotected MIN-TE      
   10.0.0.221/32              1351  721351 Node       R:0 N:1 P:0 E:0 V:0 L:0      221             L2    unprotected ADMIN       
   10.0.1.156/32               456   20456 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-156-PTX10002-36QDD L2    unprotected SPF         
   10.0.1.179/32               479   20479 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-179-ACX7024 L2    unprotected SPF         
*  10.0.30.30/32               330   20330 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-Spine3-Q2A-2-23 L2    unprotected SPF         

System ID: Arista-Spine3-Q2A-30			Instance: 'IGP'
SR supported Data-plane: MPLS			SR Router ID: 10.0.30.30

Node: 8      Proxy-Node: 0      Prefix: 0       Total Segments: 8

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
 I L2     10.0.0.32/32 [115/32]
           via 20.30.66.66, Ethernet31
 I L2     10.0.0.53/32 [115/11]
           via 20.30.66.66, Ethernet31
 I L2     10.0.0.54/32 [115/21]
           via 20.30.66.66, Ethernet31
 I L2     10.0.0.66/32 [115/11]
           via 20.30.66.66, Ethernet31
 I L2     10.0.0.72/32 [115/31]
           via 20.30.66.66, Ethernet31
 I L2     10.0.0.84/32 [115/21]
           via 20.30.66.66, Ethernet31
 I L2     10.0.0.120/32 [115/21]
           via 20.30.66.66, Ethernet31
 I L2     10.0.0.124/32 [115/21]
           via 20.30.66.66, Ethernet31
 I L2     10.0.0.128/32 [115/21]
           via 20.30.66.66, Ethernet31
 I L2     10.0.0.131/32 [115/32]
           via 20.30.66.66, Ethernet31
 I L2     10.0.0.175/32 [115/22]
           via 20.30.66.66, Ethernet31
 I L2     10.0.0.179/32 [115/23]
           via 20.30.66.66, Ethernet31
 I L2     10.0.0.185/32 [115/31]
           via 20.30.66.66, Ethernet31
 I L2     10.0.0.214/32 [115/11]
           via 20.30.66.66, Ethernet31
 I L2     10.0.0.216/32 [115/21]
           via 20.30.66.66, Ethernet31
 I L2     10.0.0.217/32 [115/32]
           via 20.30.66.66, Ethernet31
 I L2     10.0.0.221/32 [115/32]
           via 20.30.66.66, Ethernet31
 I L2     10.0.1.156/32 [115/11]
           via 20.30.66.66, Ethernet31
 I L2     10.0.1.179/32 [115/11]
           via 20.30.66.66, Ethernet31
 C        10.0.30.30/32
           directly connected, Loopback1000
 C        20.30.66.0/24
           directly connected, Ethernet31
 C        20.30.184.0/24
           directly connected, Ethernet7
 I L2     20.32.175.0/24 [115/32]
           via 20.30.66.66, Ethernet31
 I L2     20.53.66.0/24 [115/11]
           via 20.30.66.66, Ethernet31
 I L2     20.53.72.0/24 [115/21]
           via 20.30.66.66, Ethernet31
 I L2     20.53.120.0/24 [115/21]
           via 20.30.66.66, Ethernet31
 I L2     20.53.124.0/24 [115/21]
           via 20.30.66.66, Ethernet31
 I L2     20.53.128.0/24 [115/21]
           via 20.30.66.66, Ethernet31
 I L2     20.53.185.0/24 [115/21]
           via 20.30.66.66, Ethernet31
 I L2     20.53.216.0/24 [115/21]
           via 20.30.66.66, Ethernet31
 I L2     20.54.66.0/24 [115/11]
           via 20.30.66.66, Ethernet31
 I L2     20.66.84.0/24 [115/11]
           via 20.30.66.66, Ethernet31
 I L2     20.66.156.0/24 [115/11]
           via 20.30.66.66, Ethernet31
 I L2     20.66.175.0/24 [115/32]
           via 20.30.66.66, Ethernet31
 I L2     20.66.179.0/24 [115/11]
           via 20.30.66.66, Ethernet31
 I L2     20.66.214.0/24 [115/11]
           via 20.30.66.66, Ethernet31
 I L2     20.72.175.0/24 [115/32]
           via 20.30.66.66, Ethernet31
 I L2     20.120.175.0/24 [115/22]
           via 20.30.66.66, Ethernet31
 I L2     20.120.214.0/24 [115/31]
           via 20.30.66.66, Ethernet31
 I L2     20.120.217.0/24 [115/21]
           via 20.30.66.66, Ethernet31
 I L2     20.128.175.0/24 [115/32]
           via 20.30.66.66, Ethernet31
 I L2     20.131.175.0/24 [115/32]
           via 20.30.66.66, Ethernet31
 I L2     20.156.216.0/24 [115/31]
           via 20.30.66.66, Ethernet31
 I L2     20.175.179.0/24 [115/23]
           via 20.30.66.66, Ethernet31
 I L2     20.175.184.0/24 [115/32]
           via 20.30.66.66, Ethernet31
 I L2     20.175.214.0/24 [115/32]
           via 20.30.66.66, Ethernet31
 I L2     20.175.217.0/24 [115/32]
           via 20.30.66.66, Ethernet31
 I L2     20.175.221.0/24 [115/32]
           via 20.30.66.66, Ethernet31
 I L2     21.120.175.0/24 [115/23]
           via 20.30.66.66, Ethernet31
 I L2     21.175.179.0/24 [115/23]
           via 20.30.66.66, Ethernet31
 I L2     192.168.20.0/23 [115/21]
           via 20.30.66.66, Ethernet31


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
 C        50.10.30.0/24
           directly connected, Ethernet46/1.71
 B I      50.10.54.0/24 [200/0]
           via 10.0.0.54/32, IS-IS SR tunnel index 29, label 970000
              via 20.30.66.66, Ethernet31, label 20054
 B I      50.10.72.0/24 [200/0]
           via 10.0.0.72/32, IS-IS SR tunnel index 14, label 62000
              via 20.30.66.66, Ethernet31, label 20072
 B I      50.10.84.0/24 [200/0]
           via 10.0.0.84/32, IS-IS SR tunnel index 8, label 720897
              via 20.30.66.66, Ethernet31, label 20084
 B I      50.10.120.0/24 [200/0]
           via 10.0.0.120/32, IS-IS SR tunnel index 17, label 1274
              via 20.30.66.66, Ethernet31, label 20120
 B I      50.10.124.0/24 [200/0]
           via 10.0.0.124/32, IS-IS SR tunnel index 22, label 303
              via 20.30.66.66, Ethernet31, label 20124
 B I      50.10.179.0/24 [200/0]
           via 10.0.1.179/32, IS-IS SR tunnel index 23, label 30
              via 20.30.66.66, Ethernet31, label 20479
 B I      50.10.185.0/24 [200/0]
           via 10.0.0.185/32, IS-IS SR tunnel index 28, label 16
              via 20.30.66.66, Ethernet31, label 20185
 B I      50.10.214.0/24 [200/0]
           via 10.0.0.214/32, IS-IS SR tunnel index 21, label 500001
              via 20.30.66.66, Ethernet31, label 20214


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
 B I      50.128.120.0/24 [200/0]
           via 10.0.0.120/32, IS-IS SR tunnel index 17, label 1278
              via 20.30.66.66, Ethernet31, label 20120
 B I      50.128.156.0/24 [200/0]
           via 10.0.1.156/32, IS-IS SR tunnel index 24, label 17
              via 20.30.66.66, Ethernet31, label 20456
 B I      50.129.120.0/24 [200/0]
           via 10.0.0.120/32, IS-IS SR tunnel index 17, label 1277
              via 20.30.66.66, Ethernet31, label 20120
 B I      50.129.156.0/24 [200/0]
           via 10.0.1.156/32, IS-IS SR tunnel index 24, label 17
              via 20.30.66.66, Ethernet31, label 20456
 B I      50.130.120.0/24 [200/0]
           via 10.0.0.120/32, IS-IS SR tunnel index 17, label 1276
              via 20.30.66.66, Ethernet31, label 20120
 B I      50.130.156.0/24 [200/0]
           via 10.0.1.156/32, IS-IS SR tunnel index 24, label 17
              via 20.30.66.66, Ethernet31, label 20456


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
 B I      50.10.120.0/24 [200/0]
           via 10.0.0.120/32, IS-IS SR tunnel index 17, label 1275
              via 20.30.66.66, Ethernet31, label 20120
 B I      50.10.156.0/24 [200/0]
           via 10.0.1.156/32, IS-IS SR tunnel index 24, label 16
              via 20.30.66.66, Ethernet31, label 20456
 B I      50.10.179.0/24 [200/0]
           via 10.0.1.179/32, IS-IS SR tunnel index 23, label 16
              via 20.30.66.66, Ethernet31, label 20479


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
Displaying 3 of 8 IPv6 routing table entries
Source Codes:
       C - connected, S - static, K - kernel, O3 - OSPFv3,
       B - Other BGP Routes, A B - BGP Aggregate, R - RIP,
       I L1 - IS-IS level 1, I L2 - IS-IS level 2, DH - DHCP,
       NG - Nexthop Group Static Route, M - Martian,
       DP - Dynamic Policy Route, L - VRF Leaked,
       G  - gRIBI, RC - Route Cache Route,
       CL - CBF Leaked Route

 C        2001:0:30:66::/64 [0/0]
           via Ethernet31, directly connected
 C        2001:0:30:184::/64 [0/0]
           via Ethernet7, directly connected
 C        2002::30/128 [0/0]
           via Loopback0, directly connected

```

## show mpls route

```text
MPLS forwarding table (Label [metric] Vias) - 24 routes 
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
                via M, forward
                    EgressACL: apply
                    20.30.66.66 Ethernet31
 20053   A[1]
                via M, forward
                    EgressACL: apply
                    20.30.66.66 Ethernet31
 20054   A[1]
                via M, forward
                    EgressACL: apply
                    20.30.66.66 Ethernet31
 20057   A[1]
                via M, forward
                    EgressACL: apply
                    20.30.66.66 Ethernet31
 20066   A[1]
                via M, pop
                    EgressACL: apply
                    20.30.66.66 Ethernet31
 20072   A[1]
                via M, forward
                    EgressACL: apply
                    20.30.66.66 Ethernet31
 20084   A[1]
                via M, forward
                    EgressACL: apply
                    20.30.66.66 Ethernet31
 20120   A[1]
                via M, forward
                    EgressACL: apply
                    20.30.66.66 Ethernet31
 20124   A[1]
                via M, forward
                    EgressACL: apply
                    20.30.66.66 Ethernet31
 20128   A[1]
                via M, forward
                    EgressACL: apply
                    20.30.66.66 Ethernet31
 20131   A[1]
                via M, forward
                    EgressACL: apply
                    20.30.66.66 Ethernet31
 20175   A[1]
                via M, forward
                    EgressACL: apply
                    20.30.66.66 Ethernet31
 20179   A[1]
                via M, forward
                    EgressACL: apply
                    20.30.66.66 Ethernet31
 20185   A[1]
                via M, forward
                    EgressACL: apply
                    20.30.66.66 Ethernet31
 20214   A[1]
                via M, forward
                    EgressACL: apply
                    20.30.66.66 Ethernet31
 20216   A[1]
                via M, forward
                    EgressACL: apply
                    20.30.66.66 Ethernet31
 20221   A[1]
                via M, forward
                    EgressACL: apply
                    20.30.66.66 Ethernet31
 20456   A[1]
                via M, forward
                    EgressACL: apply
                    20.30.66.66 Ethernet31
 20479   A[1]
                via M, forward
                    EgressACL: apply
                    20.30.66.66 Ethernet31
 362144   [0]
                via I, ipv4, vrf FLEXALGO
 362145   [0]
                via I, ipv4, vrf RED
 362146   [0]
                via I, ipv6, vrf RED
 362147   [0]
                via I, ipv4, vrf 2-23-5G-L3VPN
 378674  A[1]
                via M, 20.30.66.66, pop
                    EgressACL: apply
                    directly connected, Ethernet31
                    e4:6d:7f:e3:c8:0a, vlan 1020
```

## show mpls lfib route

```text
MPLS forwarding table (Label [metric] Vias) - 27 routes 
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
                via M, 20.30.66.66, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet31
 IP    20053    [1], 10.0.0.53/32
                via M, 20.30.66.66, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet31
 IP    20054    [1], 10.0.0.54/32
                via M, 20.30.66.66, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet31
 IP    20057    [1], 10.0.0.217/32
                via M, 20.30.66.66, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet31
 IP    20066    [1], 10.0.0.66/32
                via M, 20.30.66.66, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet31
 IP    20072    [1], 10.0.0.72/32
                via M, 20.30.66.66, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet31
 IP    20084    [1], 10.0.0.84/32
                via M, 20.30.66.66, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet31
 IP    20120    [1], 10.0.0.120/32
                via M, 20.30.66.66, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet31
 IP    20124    [1], 10.0.0.124/32
                via M, 20.30.66.66, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet31
 IP    20128    [1], 10.0.0.128/32
                via M, 20.30.66.66, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet31
 IP    20131    [1], 10.0.0.131/32
                via M, 20.30.66.66, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet31
 IP    20175    [1], 10.0.0.175/32
                via M, 20.30.66.66, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet31
 IP    20179    [1], 10.0.0.179/32
                via M, 20.30.66.66, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet31
 IP    20185    [1], 10.0.0.185/32
                via M, 20.30.66.66, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet31
 IP    20214    [1], 10.0.0.214/32
                via M, 20.30.66.66, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet31
 IP    20216    [1], 10.0.0.216/32
                via M, 20.30.66.66, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet31
 IP    20221    [1], 10.0.0.221/32
                via M, 20.30.66.66, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet31
 IP    20456    [1], 10.0.1.156/32
                via M, 20.30.66.66, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet31
 IP    20479    [1], 10.0.1.179/32
                via M, 20.30.66.66, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet31
 B3    362144   [0]
                via I, ipv4, vrf FLEXALGO
 B3    362145   [0]
                via I, ipv4, vrf RED
 B3    362146   [0]
                via I, ipv6, vrf RED
 B3    362147   [0]
                via I, ipv4, vrf 2-23-5G-L3VPN
 IA    378674   [1]
                via M, 20.30.66.66, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet31
 P     411296   [1]
                 via VP, patch 2-23-5G-NOKIA-214-PATCH_PANEL
                  interface Ethernet46/1.1214, type 5
 P     411298   [1]
                 via VP, patch 2-23-5G-JUNIPER-179-PATCH_PANEL
                  interface Ethernet46/1.1179, type 5
 P     411299   [1]
                 via VP, patch 2-23-5G-H3C-120-PATCH_PANEL
                  interface Ethernet46/1.1120, type 5
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
 * >      RD: 10.0.30.30:1030 auto-discovery 30 0000:0000:0000:0000:0000
                                 -                     -       -       0       i
 * >      RD: 10.0.30.30:2030 auto-discovery 30 0000:0000:0000:0000:0000
                                 -                     -       -       0       i
 * >Ec    RD: 10.0.0.72:2 auto-discovery 72 0000:0000:0000:0000:0000
                                 10.0.0.72             -       100     0       i Or-ID: 10.0.0.72 C-LST: 10.0.0.216 
 *  ec    RD: 10.0.0.72:2 auto-discovery 72 0000:0000:0000:0000:0000
                                 10.0.0.72             -       100     0       i Or-ID: 10.0.0.72 C-LST: 10.0.1.156 
 * >Ec    RD: 10.0.0.72:5 auto-discovery 72 0000:0000:0000:0000:0000
                                 10.0.0.72             -       100     0       i Or-ID: 10.0.0.72 C-LST: 10.0.0.216 
 *  ec    RD: 10.0.0.72:5 auto-discovery 72 0000:0000:0000:0000:0000
                                 10.0.0.72             -       100     0       i Or-ID: 10.0.0.72 C-LST: 10.0.1.156 
 * >Ec    RD: 684:6179 auto-discovery 84 0000:0000:0000:0000:0000
                                 10.0.0.84             0       100     0       ? Or-ID: 10.0.0.84 C-LST: 10.0.0.216 
 *  ec    RD: 684:6179 auto-discovery 84 0000:0000:0000:0000:0000
                                 10.0.0.84             0       100     0       ? Or-ID: 10.0.0.84 C-LST: 10.0.1.156 
 * >      RD: 120:6214 auto-discovery 120 0000:0000:0000:0000:0000
                                 10.0.0.120            0       100     0       i Or-ID: 10.0.0.120 C-LST: 10.0.0.216 
 * >      RD: 6124:124 auto-discovery 124 0000:0000:0000:0000:0000
                                 10.0.0.124            -       100     0       i Or-ID: 10.0.0.124 C-LST: 10.0.0.216 
 * >Ec    RD: 6001:128 auto-discovery 128 0000:0000:0000:0000:0000
                                 10.0.0.128            -       100     0       i Or-ID: 10.0.0.128 C-LST: 10.0.0.216 
 *  ec    RD: 6001:128 auto-discovery 128 0000:0000:0000:0000:0000
                                 10.0.0.128            -       100     0       i Or-ID: 10.0.0.128 C-LST: 10.0.1.156 
 * >Ec    RD: 10.0.0.179:65531 auto-discovery 179 0000:0000:0000:0000:0000
                                 10.0.1.179            -       100     0       i Or-ID: 10.0.0.179 C-LST: 10.0.0.216 
 *  ec    RD: 10.0.0.179:65531 auto-discovery 179 0000:0000:0000:0000:0000
                                 10.0.1.179            -       100     0       i Or-ID: 10.0.0.179 C-LST: 10.0.1.156 
 * >Ec    RD: 10.0.0.179:65532 auto-discovery 179 0000:0000:0000:0000:0000
                                 10.0.1.179            -       100     0       i Or-ID: 10.0.0.179 C-LST: 10.0.0.216 
 *  ec    RD: 10.0.0.179:65532 auto-discovery 179 0000:0000:0000:0000:0000
                                 10.0.1.179            -       100     0       i Or-ID: 10.0.0.179 C-LST: 10.0.1.156 
 * >Ec    RD: 10.0.0.179:65533 auto-discovery 179 0000:0000:0000:0000:0000
                                 10.0.1.179            -       100     0       i Or-ID: 10.0.0.179 C-LST: 10.0.0.216 
 *  ec    RD: 10.0.0.179:65533 auto-discovery 179 0000:0000:0000:0000:0000
                                 10.0.1.179            -       100     0       i Or-ID: 10.0.0.179 C-LST: 10.0.1.156 
 * >Ec    RD: 10.0.0.179:65534 auto-discovery 179 0000:0000:0000:0000:0000
                                 10.0.1.179            -       100     0       i Or-ID: 10.0.0.179 C-LST: 10.0.0.216 
 *  ec    RD: 10.0.0.179:65534 auto-discovery 179 0000:0000:0000:0000:0000
                                 10.0.1.179            -       100     0       i Or-ID: 10.0.0.179 C-LST: 10.0.1.156 
 * >Ec    RD: 214:54 auto-discovery 214 0000:0000:0000:0000:0000
                                 10.0.0.214            -       100     0       i Or-ID: 10.0.0.214 C-LST: 10.0.0.216 
 *  ec    RD: 214:54 auto-discovery 214 0000:0000:0000:0000:0000
                                 10.0.0.214            -       100     0       i Or-ID: 10.0.0.214 C-LST: 10.0.1.156 
 * >Ec    RD: 214:124 auto-discovery 214 0000:0000:0000:0000:0000
                                 10.0.0.214            -       100     0       i Or-ID: 10.0.0.214 C-LST: 10.0.0.216 
 *  ec    RD: 214:124 auto-discovery 214 0000:0000:0000:0000:0000
                                 10.0.0.214            -       100     0       i Or-ID: 10.0.0.214 C-LST: 10.0.1.156 
 * >Ec    RD: 214:179 auto-discovery 214 0000:0000:0000:0000:0000
                                 10.0.0.214            -       100     0       i Or-ID: 10.0.0.214 C-LST: 10.0.0.216 
 *  ec    RD: 214:179 auto-discovery 214 0000:0000:0000:0000:0000
                                 10.0.0.214            -       100     0       i Or-ID: 10.0.0.214 C-LST: 10.0.1.156 
 * >Ec    RD: 10.0.0.214:120 auto-discovery 214 0000:0000:0000:0000:0000
                                 10.0.0.214            -       100     0       i Or-ID: 10.0.0.214 C-LST: 10.0.0.216 
 *  ec    RD: 10.0.0.214:120 auto-discovery 214 0000:0000:0000:0000:0000
                                 10.0.0.214            -       100     0       i Or-ID: 10.0.0.214 C-LST: 10.0.1.156 
 * >Ec    RD: 10.0.0.214:130 auto-discovery 214 0000:0000:0000:0000:0000
                                 10.0.0.214            -       100     0       i Or-ID: 10.0.0.214 C-LST: 10.0.0.216 
 *  ec    RD: 10.0.0.214:130 auto-discovery 214 0000:0000:0000:0000:0000
                                 10.0.0.214            -       100     0       i Or-ID: 10.0.0.214 C-LST: 10.0.1.156 
 * >Ec    RD: 10.0.0.214:6001 auto-discovery 214 0000:0000:0000:0000:0000
                                 10.0.0.214            -       100     0       i Or-ID: 10.0.0.214 C-LST: 10.0.0.216 
 *  ec    RD: 10.0.0.214:6001 auto-discovery 214 0000:0000:0000:0000:0000
                                 10.0.0.214            -       100     0       i Or-ID: 10.0.0.214 C-LST: 10.0.1.156 
 * >Ec    RD: 10.0.0.54:2056 auto-discovery 454 0000:0000:0000:0000:0000
                                 10.0.0.54             -       100     0       i Or-ID: 10.0.0.54 C-LST: 10.0.0.216 
 *  ec    RD: 10.0.0.54:2056 auto-discovery 454 0000:0000:0000:0000:0000
                                 10.0.0.54             -       100     0       i Or-ID: 10.0.0.54 C-LST: 10.0.1.156 
 * >Ec    RD: 10.0.0.72:3 auto-discovery 672 0000:0000:0000:0000:0000
                                 10.0.0.72             -       100     0       i Or-ID: 10.0.0.72 C-LST: 10.0.0.216 
 *  ec    RD: 10.0.0.72:3 auto-discovery 672 0000:0000:0000:0000:0000
                                 10.0.0.72             -       100     0       i Or-ID: 10.0.0.72 C-LST: 10.0.1.156 
 * >Ec    RD: 684:630 auto-discovery 684 0000:0000:0000:0000:0000
                                 10.0.0.84             0       100     0       ? Or-ID: 10.0.0.84 C-LST: 10.0.0.216 
 *  ec    RD: 684:630 auto-discovery 684 0000:0000:0000:0000:0000
                                 10.0.0.84             0       100     0       ? Or-ID: 10.0.0.84 C-LST: 10.0.1.156 
 * >Ec    RD: 684:654 auto-discovery 684 0000:0000:0000:0000:0000
                                 10.0.0.84             0       100     0       ? Or-ID: 10.0.0.84 C-LST: 10.0.0.216 
 *  ec    RD: 684:654 auto-discovery 684 0000:0000:0000:0000:0000
                                 10.0.0.84             0       100     0       ? Or-ID: 10.0.0.84 C-LST: 10.0.1.156 
 * >Ec    RD: 684:672 auto-discovery 684 0000:0000:0000:0000:0000
                                 10.0.0.84             0       100     0       ? Or-ID: 10.0.0.84 C-LST: 10.0.0.216 
 *  ec    RD: 684:672 auto-discovery 684 0000:0000:0000:0000:0000
                                 10.0.0.84             0       100     0       ? Or-ID: 10.0.0.84 C-LST: 10.0.1.156 
 * >Ec    RD: 684:6120 auto-discovery 684 0000:0000:0000:0000:0000
                                 10.0.0.84             0       100     0       ? Or-ID: 10.0.0.84 C-LST: 10.0.0.216 
 *  ec    RD: 684:6120 auto-discovery 684 0000:0000:0000:0000:0000
                                 10.0.0.84             0       100     0       ? Or-ID: 10.0.0.84 C-LST: 10.0.1.156 
 * >Ec    RD: 684:6124 auto-discovery 684 0000:0000:0000:0000:0000
                                 10.0.0.84             0       100     0       ? Or-ID: 10.0.0.84 C-LST: 10.0.0.216 
 *  ec    RD: 684:6124 auto-discovery 684 0000:0000:0000:0000:0000
                                 10.0.0.84             0       100     0       ? Or-ID: 10.0.0.84 C-LST: 10.0.1.156 
 * >Ec    RD: 684:6128 auto-discovery 684 0000:0000:0000:0000:0000
                                 10.0.0.84             0       100     0       ? Or-ID: 10.0.0.84 C-LST: 10.0.0.216 
 *  ec    RD: 684:6128 auto-discovery 684 0000:0000:0000:0000:0000
                                 10.0.0.84             0       100     0       ? Or-ID: 10.0.0.84 C-LST: 10.0.1.156 
 * >Ec    RD: 684:6174 auto-discovery 684 0000:0000:0000:0000:0000
                                 10.0.0.84             0       100     0       ? Or-ID: 10.0.0.84 C-LST: 10.0.0.216 
 *  ec    RD: 684:6174 auto-discovery 684 0000:0000:0000:0000:0000
                                 10.0.0.84             0       100     0       ? Or-ID: 10.0.0.84 C-LST: 10.0.1.156 
 * >Ec    RD: 684:6214 auto-discovery 684 0000:0000:0000:0000:0000
                                 10.0.0.84             0       100     0       ? Or-ID: 10.0.0.84 C-LST: 10.0.0.216 
 *  ec    RD: 684:6214 auto-discovery 684 0000:0000:0000:0000:0000
                                 10.0.0.84             0       100     0       ? Or-ID: 10.0.0.84 C-LST: 10.0.1.156 
 * >Ec    RD: 10.0.0.54:2055 auto-discovery 1054 0000:0000:0000:0000:0000
                                 10.0.0.54             -       100     0       i Or-ID: 10.0.0.54 C-LST: 10.0.0.216 
 *  ec    RD: 10.0.0.54:2055 auto-discovery 1054 0000:0000:0000:0000:0000
                                 10.0.0.54             -       100     0       i Or-ID: 10.0.0.54 C-LST: 10.0.1.156 
 * >Ec    RD: 10.0.0.72:4 auto-discovery 1072 0000:0000:0000:0000:0000
                                 10.0.0.72             -       100     0       i Or-ID: 10.0.0.72 C-LST: 10.0.0.216 
 *  ec    RD: 10.0.0.72:4 auto-discovery 1072 0000:0000:0000:0000:0000
                                 10.0.0.72             -       100     0       i Or-ID: 10.0.0.72 C-LST: 10.0.1.156 
          RD: 10.0.0.216:1122 auto-discovery 1122 0000:0000:0000:0000:0000
                                 2002::216             -       100     0       i
          RD: 10.0.0.216:1222 auto-discovery 1222 0000:0000:0000:0000:0000
                                 2002::216             -       100     0       i
          RD: 10.0.0.216:1322 auto-discovery 1322 0000:0000:0000:0000:0000
                                 2002::216             -       100     0       i
          RD: 10.0.0.216:1422 auto-discovery 1422 0000:0000:0000:0000:0000
                                 2002::216             -       100     0       i
          RD: 10.0.0.216:1522 auto-discovery 1522 0000:0000:0000:0000:0000
                                 2002::216             -       100     0       i
          RD: 10.0.0.216:1622 auto-discovery 1622 0000:0000:0000:0000:0000
                                 2002::216             -       100     0       i
          RD: 10.0.0.216:1722 auto-discovery 1722 0000:0000:0000:0000:0000
                                 2002::216             -       100     0       i
          RD: 10.0.0.216:1822 auto-discovery 1822 0000:0000:0000:0000:0000
                                 2002::216             -       100     0       i
          RD: 10.0.0.216:1922 auto-discovery 1922 0000:0000:0000:0000:0000
                                 2002::216             -       100     0       i
          RD: 10.0.0.216:2022 auto-discovery 2022 0000:0000:0000:0000:0000
                                 2002::216             -       100     0       i
 * >      RD: 10.0.30.30:6001 auto-discovery 2030 0000:0000:0000:0000:0000
                                 -                     -       -       0       i
 * >Ec    RD: 10.0.0.54:2054 auto-discovery 2054 0000:0000:0000:0000:0000
                                 10.0.0.54             -       100     0       i Or-ID: 10.0.0.54 C-LST: 10.0.0.216 
 *  ec    RD: 10.0.0.54:2054 auto-discovery 2054 0000:0000:0000:0000:0000
                                 10.0.0.54             -       100     0       i Or-ID: 10.0.0.54 C-LST: 10.0.1.156 
 * >Ec    RD: 10.0.0.72:1 auto-discovery 2072 0000:0000:0000:0000:0000
                                 10.0.0.72             -       100     0       i Or-ID: 10.0.0.72 C-LST: 10.0.0.216 
 *  ec    RD: 10.0.0.72:1 auto-discovery 2072 0000:0000:0000:0000:0000
                                 10.0.0.72             -       100     0       i Or-ID: 10.0.0.72 C-LST: 10.0.1.156 
 * >      RD: 120:6001 auto-discovery 2120 0000:0000:0000:0000:0000
                                 10.0.0.120            0       100     0       i Or-ID: 10.0.0.120 C-LST: 10.0.0.216 
          RD: 10.0.0.216:2122 auto-discovery 2122 0000:0000:0000:0000:0000
                                 2002::216             -       100     0       i
 * >      RD: 10.0.0.185:185 auto-discovery 2185 0000:0000:0000:0000:0000
                                 10.0.0.185            -       0       0       i Or-ID: 192.0.0.1 C-LST: 10.0.0.216 
          RD: 10.0.0.216:2223 auto-discovery 2223 0000:0000:0000:0000:0000
                                 2002::216             -       100     0       i
          RD: 10.0.0.216:50 mac-ip 0050.0100.0216
                                 2002::216             -       100     0       i
          RD: 10.0.0.216:50 imet 2002::216
                                 2002::216             -       100     0       i
 * >      RD: 10.0.0.216:40 ip-prefix 40.190.216.0/24
                                 10.0.0.216            -       100     0       i
 * >      RD: 10.0.0.216:42 ip-prefix 42.190.216.0/24
                                 10.0.0.216            -       100     0       i
 * >Ec    RD: 54:7001 ip-prefix 50.10.54.0/24
                                 10.0.0.54             -       100     0       ? Or-ID: 10.0.0.54 C-LST: 10.0.0.216 
 *  ec    RD: 54:7001 ip-prefix 50.10.54.0/24
                                 10.0.0.54             -       100     0       ? Or-ID: 10.0.0.54 C-LST: 10.0.1.156 
 * >      RD: 10.0.0.216:40 ip-prefix 2600:40:190:216::/64
                                 10.0.0.216            -       100     0       i
 * >      RD: 10.0.0.216:42 ip-prefix 2600:42:190:216::/64
                                 10.0.0.216            -       100     0       i
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
 * >      RD: 10.0.30.30:7001 IPv4 prefix 10.0.30.30/32
                                 -                     -       -       0       i
 * >      RD: 10.0.0.216:20 IPv4 prefix 20.190.216.0/24
                                 10.0.0.216            -       100     0       i
 * >      RD: 10.0.0.216:22 IPv4 prefix 22.190.216.0/24
                                 10.0.0.216            -       100     0       i
 * >      RD: 10.0.30.30:7001 IPv4 prefix 50.10.30.0/24
                                 -                     -       -       0       i
 * >Ec    RD: 54:7001 IPv4 prefix 50.10.54.0/24
                                 10.0.0.54             -       100     0       ? Or-ID: 10.0.0.54 C-LST: 10.0.0.216 
 *  ec    RD: 54:7001 IPv4 prefix 50.10.54.0/24
                                 10.0.0.54             -       100     0       ? Or-ID: 10.0.0.54 C-LST: 10.0.1.156 
 * >Ec    RD: 72:7001 IPv4 prefix 50.10.72.0/24
                                 10.0.0.72             -       100     0       ? Or-ID: 10.0.0.72 C-LST: 10.0.0.216 
 *  ec    RD: 72:7001 IPv4 prefix 50.10.72.0/24
                                 10.0.0.72             -       100     0       ? Or-ID: 10.0.0.72 C-LST: 10.0.1.156 
 * >Ec    RD: 184:5001 IPv4 prefix 50.10.84.0/24
                                 10.0.0.84             0       100     0       ? Or-ID: 10.0.0.84 C-LST: 10.0.0.216 
 *  ec    RD: 184:5001 IPv4 prefix 50.10.84.0/24
                                 10.0.0.84             0       100     0       ? Or-ID: 10.0.0.84 C-LST: 10.0.1.156 
 * >Ec    RD: 120:5001 IPv4 prefix 50.10.120.0/24
                                 10.0.0.120            0       100     0       ? Or-ID: 10.0.0.120 C-LST: 10.0.0.216 
 *  ec    RD: 120:5001 IPv4 prefix 50.10.120.0/24
                                 10.0.0.120            0       100     0       ? Or-ID: 10.0.0.120 C-LST: 10.0.1.156 
 * >Ec    RD: 120:7001 IPv4 prefix 50.10.120.0/24
                                 10.0.0.120            0       100     0       ? Or-ID: 10.0.0.120 C-LST: 10.0.0.216 
 *  ec    RD: 120:7001 IPv4 prefix 50.10.120.0/24
                                 10.0.0.120            0       100     0       ? Or-ID: 10.0.0.120 C-LST: 10.0.1.156 
 * >      RD: 7001:124 IPv4 prefix 50.10.124.0/24
                                 10.0.0.124            0       100     0       ? Or-ID: 10.0.0.124 C-LST: 10.0.0.216 
 * >      RD: 156:5001 IPv4 prefix 50.10.156.0/24
                                 10.0.1.156            -       100     0       i
 * >Ec    RD: 179:5001 IPv4 prefix 50.10.179.0/24
                                 10.0.1.179            -       100     0       i Or-ID: 10.0.0.179 C-LST: 10.0.0.216 
 *  ec    RD: 179:5001 IPv4 prefix 50.10.179.0/24
                                 10.0.1.179            -       100     0       i Or-ID: 10.0.0.179 C-LST: 10.0.1.156 
 * >Ec    RD: 10.0.0.179:57 IPv4 prefix 50.10.179.0/24
                                 10.0.1.179            -       100     0       i Or-ID: 10.0.0.179 C-LST: 10.0.0.216 
 *  ec    RD: 10.0.0.179:57 IPv4 prefix 50.10.179.0/24
                                 10.0.1.179            -       100     0       i Or-ID: 10.0.0.179 C-LST: 10.0.1.156 
 * >      RD: 185:7001 IPv4 prefix 50.10.185.0/24
                                 10.0.0.185            -       0       0       i Or-ID: 192.0.0.1 C-LST: 10.0.0.216 
 * >Ec    RD: 214:7001 IPv4 prefix 50.10.214.0/24
                                 10.0.0.214            -       100     0       i Or-ID: 10.0.0.214 C-LST: 10.0.0.216 
 *  ec    RD: 214:7001 IPv4 prefix 50.10.214.0/24
                                 10.0.0.214            -       100     0       i Or-ID: 10.0.0.214 C-LST: 10.0.1.156 
 * >Ec    RD: 120:5128 IPv4 prefix 50.128.120.0/24
                                 10.0.0.120            0       100     0       ? Or-ID: 10.0.0.120 C-LST: 10.0.0.216 
 *  ec    RD: 120:5128 IPv4 prefix 50.128.120.0/24
                                 10.0.0.120            0       100     0       ? Or-ID: 10.0.0.120 C-LST: 10.0.1.156 
 * >      RD: 5128:5128 IPv4 prefix 50.128.156.0/24
                                 10.0.1.156            -       100     0       i
 * >Ec    RD: 120:5129 IPv4 prefix 50.129.120.0/24
                                 10.0.0.120            0       100     0       ? Or-ID: 10.0.0.120 C-LST: 10.0.0.216 
 *  ec    RD: 120:5129 IPv4 prefix 50.129.120.0/24
                                 10.0.0.120            0       100     0       ? Or-ID: 10.0.0.120 C-LST: 10.0.1.156 
 * >      RD: 5128:5128 IPv4 prefix 50.129.156.0/24
                                 10.0.1.156            -       100     0       i
 * >Ec    RD: 120:5130 IPv4 prefix 50.130.120.0/24
                                 10.0.0.120            0       100     0       ? Or-ID: 10.0.0.120 C-LST: 10.0.0.216 
 *  ec    RD: 120:5130 IPv4 prefix 50.130.120.0/24
                                 10.0.0.120            0       100     0       ? Or-ID: 10.0.0.120 C-LST: 10.0.1.156 
 * >      RD: 5128:5128 IPv4 prefix 50.130.156.0/24
                                 10.0.1.156            -       100     0       i
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
  Connect timer is active, time left: 00:00:16
  Connection interval is 148 seconds
  Failed connection attempts is 2382
  Idle-restart timer is inactive
  BGP state is Active
  Number of transitions to established: 0
  Last state was Connect
  Last event was TransportError
  Last sent socket-error:Connect (Network is unreachable), Last time 00:02:36, First time 4d16h, Repeats 2381
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
  Last read 18:25:42, last write 18:22:42
  Hold time is 180, keepalive interval is 60 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is inactive
  Keepalive timer is inactive
  Connect timer is active, time left: 00:00:16
  Connection interval is 20 seconds
  Failed connection attempts is 2845
  Idle-restart timer is inactive
  BGP state is Connect
  Number of transitions to established: 2
  Last state was Active
  Last event was ConnectRetry
  Last sent notification:Hold Timer Expired Error/None, Last time 18:22:42
  Last sent socket-error:Connect (Network is unreachable), Last time 18:07:50, First time 18:21:52, Repeats 10
  Types of communities advertised: standard extended large
  Neighbor is a route reflector client
  Neighbor is using global cluster ID 10.0.0.30
  Neighbor Capabilities:
    Multiprotocol VPN-IPv4: advertised and received
    Multiprotocol VPN-IPv6: advertised and received
    Four Octet ASN: advertised and received
    Route Refresh: advertised and received
    Enhanced route refresh: advertised and received
    Send End-of-RIB messages: advertised and received
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
    Opens:                  2         2
    Notifications:          1         0
    Updates:              479        14
    Keepalives:          6546      6610
    Route Refresh:          0         0
    Total messages:      7028      6626
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
Remote TCP address is 10.0.0.32, remote port is 179
TCP Socket Information:
  TCP state is SYN-SENT
  Recv-Q: 0/131072
  Send-Q: 0/16384
  Outgoing Maximum Segment Size (MSS): 524
  Total Number of TCP retransmissions: 2
  Options:
    Timestamps enabled: no
    Selective Acknowledgments enabled: no
    Window Scale enabled: no
    Explicit Congestion Notification (ECN) enabled: no
  Socket Statistics:
    Window Scale (wscale): 0,0
    Retransmission Timeout (rto): 4000.0ms
    Round-trip Time (rtt/rtvar): 0.0ms/250.0ms
    Delayed Ack Timeout (ato): 0.0ms
    Congestion Window (cwnd): 1
    Slow-start Threshold (ssthresh): 7

BGP neighbor is 10.0.0.53, remote AS 64512, internal link
 Description: Arrcus-53
  BGP version 4, remote router ID 10.0.0.53, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 18:25:36, last write 18:22:36
  Hold time is 180, keepalive interval is 60 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is inactive
  Keepalive timer is inactive
  Connect timer is active, time left: 00:00:04
  Connection interval is 20 seconds
  Failed connection attempts is 2883
  Idle-restart timer is inactive
  BGP state is Connect
  Number of transitions to established: 5
  Last state was Active
  Last event was ConnectRetry
  Last sent notification:Hold Timer Expired Error/None, Last time 18:22:36, First time 19:59:51, Repeats 4
  Last sent socket-error:Connect (Network is unreachable), Last time 18:53:06, First time 19:59:50, Repeats 30
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
    Opens:                  5         5
    Notifications:          5         0
    Updates:              596        18
    Keepalives:          6479      5541
    Route Refresh:          0         2
    Total messages:      7085      5566
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
Remote TCP address is 10.0.0.53, remote port is 179
TCP Socket Information:
  TCP state is SYN-SENT
  Recv-Q: 0/131072
  Send-Q: 0/16384
  Outgoing Maximum Segment Size (MSS): 524
  Total Number of TCP retransmissions: 4
  Options:
    Timestamps enabled: no
    Selective Acknowledgments enabled: no
    Window Scale enabled: no
    Explicit Congestion Notification (ECN) enabled: no
  Socket Statistics:
    Window Scale (wscale): 0,0
    Retransmission Timeout (rto): 16000.0ms
    Round-trip Time (rtt/rtvar): 0.0ms/250.0ms
    Delayed Ack Timeout (ato): 0.0ms
    Congestion Window (cwnd): 1
    Slow-start Threshold (ssthresh): 7

BGP neighbor is 10.0.0.66, remote AS 64512, internal link
 Description: Ciena-8140-66
  BGP version 4, remote router ID 10.0.0.66, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 21:02:57, last write 18:28:09
  Hold time is 180, keepalive interval is 60 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is inactive
  Keepalive timer is inactive
  Connect timer is active, time left: 00:00:03
  Connection interval is 20 seconds
  Failed connection attempts is 2885
  Idle-restart timer is inactive
  BGP state is Connect
  Number of transitions to established: 7
  Last state was Active
  Last event was ConnectRetry
  Last sent notification:Hold Timer Expired Error/None, Last time 20:59:57, First time 3d23h, Repeats 2
  Last rcvd notification:Cease/other configuration change, Last time 23:53:19, First time 4d15h, Repeats 3
  Last sent socket-error:Connect (Connection refused), Last time 18:33:37
  Last rcvd socket-error:Connection reset by peer, Last time 18:28:09, First time 3d18h, Repeats 4
  Types of communities advertised: standard extended large
  Neighbor is a route reflector client
  Neighbor is using global cluster ID 10.0.0.30
  Neighbor Capabilities:
    Multiprotocol IPv4 Unicast: received
    Multiprotocol VPN-IPv4: advertised and received
    Multiprotocol VPN-IPv6: advertised
    Four Octet ASN: advertised
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
      Restart-time is 0
      Restart-State bit: no
      Graceful notification: no
      IPv4 Unicast is enabled, Forwarding State is not preserved
      VPN-IPv4 is enabled, Forwarding State is not preserved
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
    Opens:                 12         7
    Notifications:          3         4
    Updates:              442        24
    Keepalives:          6186      5280
    Route Refresh:          0         0
    Total messages:      6643      5315
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
Remote TCP address is 10.0.0.66, remote port is 179
TCP Socket Information:
  TCP state is SYN-SENT
  Recv-Q: 0/131072
  Send-Q: 0/16384
  Outgoing Maximum Segment Size (MSS): 524
  Total Number of TCP retransmissions: 4
  Options:
    Timestamps enabled: no
    Selective Acknowledgments enabled: no
    Window Scale enabled: no
    Explicit Congestion Notification (ECN) enabled: no
  Socket Statistics:
    Window Scale (wscale): 0,0
    Retransmission Timeout (rto): 16000.0ms
    Round-trip Time (rtt/rtvar): 0.0ms/250.0ms
    Delayed Ack Timeout (ato): 0.0ms
    Congestion Window (cwnd): 1
    Slow-start Threshold (ssthresh): 7

BGP neighbor is 10.0.0.72, remote AS 64512, internal link
 Description: Ciena-5134-72
  BGP version 4, remote router ID 10.0.0.72, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 21:02:19, last write 21:02:26
  Hold time is 180, keepalive interval is 60 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is inactive
  Keepalive timer is inactive
  Connect timer is active, time left: 00:00:00
  Connection interval is 20 seconds
  Failed connection attempts is 2830
  Idle-restart timer is inactive
  BGP state is Connect
  Number of transitions to established: 9
  Last state was Active
  Last event was ConnectRetry
  Last sent notification:Hold Timer Expired Error/None, Last time 3d19h, First time 3d23h, Repeats 1
  Last rcvd notification:Cease/other configuration change, Last time 21:02:19, First time 4d16h, Repeats 6
  Last sent socket-error:Connect (Network is unreachable), Last time 18:05:11, First time 21:01:53, Repeats 67
  Last rcvd socket-error:Connection reset by peer, Last time 23:54:50, First time 3d20h, Repeats 5
  Types of communities advertised: standard extended large
  Neighbor is a route reflector client
  Neighbor is using global cluster ID 10.0.0.30
  Neighbor Capabilities:
    Multiprotocol IPv4 Unicast: received
    Multiprotocol VPN-IPv4: advertised and received
    Multiprotocol VPN-IPv6: advertised
    Four Octet ASN: advertised
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
      Restart-time is 0
      Restart-State bit: no
      Graceful notification: no
      IPv4 Unicast is enabled, Forwarding State is not preserved
      VPN-IPv4 is enabled, Forwarding State is not preserved
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
    Opens:                 15         9
    Notifications:          2         7
    Updates:              491        29
    Keepalives:          6177      5277
    Route Refresh:          0         0
    Total messages:      6685      5322
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
Remote TCP address is 10.0.0.72, remote port is 179
TCP Socket Information:
  TCP state is SYN-SENT
  Recv-Q: 0/131072
  Send-Q: 0/16384
  Outgoing Maximum Segment Size (MSS): 524
  Total Number of TCP retransmissions: 4
  Options:
    Timestamps enabled: no
    Selective Acknowledgments enabled: no
    Window Scale enabled: no
    Explicit Congestion Notification (ECN) enabled: no
  Socket Statistics:
    Window Scale (wscale): 0,0
    Retransmission Timeout (rto): 16000.0ms
    Round-trip Time (rtt/rtvar): 0.0ms/250.0ms
    Delayed Ack Timeout (ato): 0.0ms
    Congestion Window (cwnd): 1
    Slow-start Threshold (ssthresh): 7

BGP neighbor is 10.0.0.84, remote AS 64512, internal link
 Description: Ericsson_84
  BGP version 4, remote router ID 10.0.0.84, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 19:53:40, last write 19:50:40
  Hold time is 180, keepalive interval is 60 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is inactive
  Keepalive timer is inactive
  Connect timer is active, time left: 00:00:04
  Connection interval is 20 seconds
  Failed connection attempts is 2881
  Idle-restart timer is inactive
  BGP state is Connect
  Number of transitions to established: 1
  Last state was Active
  Last event was ConnectRetry
  Last sent notification:Hold Timer Expired Error/None, Last time 19:50:40
  Last sent socket-error:Connect (Network is unreachable), Last time 18:57:55, First time 19:50:38, Repeats 27
  Types of communities advertised: standard extended large
  Neighbor is a route reflector client
  Neighbor is using global cluster ID 10.0.0.30
  Neighbor Capabilities:
    Multiprotocol IPv4 Unicast: received
    Multiprotocol VPN-IPv4: advertised and received
    Multiprotocol IPv6 Unicast: received
    Multiprotocol VPN-IPv6: advertised and received
    Multiprotocol L2VPN EVPN: received
    Four Octet ASN: advertised and received
    Route Refresh: advertised and received
    Enhanced route refresh: advertised and received
    Send End-of-RIB messages: advertised and received
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
    Notifications:          1         0
    Updates:              362         4
    Keepalives:          6464      5528
    Route Refresh:          0         0
    Total messages:      6828      5533
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
Remote TCP address is 10.0.0.84, remote port is 179
TCP Socket Information:
  TCP state is SYN-SENT
  Recv-Q: 0/131072
  Send-Q: 0/16384
  Outgoing Maximum Segment Size (MSS): 524
  Total Number of TCP retransmissions: 4
  Options:
    Timestamps enabled: no
    Selective Acknowledgments enabled: no
    Window Scale enabled: no
    Explicit Congestion Notification (ECN) enabled: no
  Socket Statistics:
    Window Scale (wscale): 0,0
    Retransmission Timeout (rto): 16000.0ms
    Round-trip Time (rtt/rtvar): 0.0ms/250.0ms
    Delayed Ack Timeout (ato): 0.0ms
    Congestion Window (cwnd): 1
    Slow-start Threshold (ssthresh): 7

BGP neighbor is 10.0.0.120, remote AS 64512, internal link
 Description: Huawei_120
  BGP version 4, remote router ID 10.0.0.120, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 18:26:02, last write 18:23:02
  Hold time is 180, keepalive interval is 60 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is inactive
  Keepalive timer is inactive
  Connect timer is active, time left: 00:00:00
  Connection interval is 20 seconds
  Failed connection attempts is 2845
  Idle-restart timer is inactive
  BGP state is Connect
  Number of transitions to established: 9
  Last state was Active
  Last event was ConnectRetry
  Last sent notification:Hold Timer Expired Error/None, Last time 18:23:02, First time 18:37:09, Repeats 1
  Last rcvd notification:Cease/connection collision resolution, Last time 19:46:37
  Last sent socket-error:Connect (Network is unreachable), Last time 18:07:50, First time 18:21:53, Repeats 9
  Last rcvd socket-error:Connection reset by peer, Last time 18:43:26, First time 18:46:39, Repeats 1
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
Local TCP address is 10.0.0.30
Remote TCP address is 10.0.0.120, remote port is 179
TCP Socket Information:
  TCP state is SYN-SENT
  Recv-Q: 0/131072
  Send-Q: 0/16384
  Outgoing Maximum Segment Size (MSS): 524
  Total Number of TCP retransmissions: 4
  Options:
    Timestamps enabled: no
    Selective Acknowledgments enabled: no
    Window Scale enabled: no
    Explicit Congestion Notification (ECN) enabled: no
  Socket Statistics:
    Window Scale (wscale): 0,0
    Retransmission Timeout (rto): 16000.0ms
    Round-trip Time (rtt/rtvar): 0.0ms/250.0ms
    Delayed Ack Timeout (ato): 0.0ms
    Congestion Window (cwnd): 1
    Slow-start Threshold (ssthresh): 7

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
  Connect timer is active, time left: 00:00:03
  Connection interval is 20 seconds
  Failed connection attempts is 205
  Idle-restart timer is inactive
  BGP state is Connect
  Number of transitions to established: 0
  Last state was Active
  Last event was ConnectRetry
  Last sent socket-error:Connect (Network is unreachable), Last time 01:19:43, First time 18:23:52, Repeats 6
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
TCP Socket Information:
  TCP state is SYN-SENT
  Recv-Q: 0/131072
  Send-Q: 0/16384
  Outgoing Maximum Segment Size (MSS): 524
  Total Number of TCP retransmissions: 4
  Options:
    Timestamps enabled: no
    Selective Acknowledgments enabled: no
    Window Scale enabled: no
    Explicit Congestion Notification (ECN) enabled: no
  Socket Statistics:
    Window Scale (wscale): 0,0
    Retransmission Timeout (rto): 16000.0ms
    Round-trip Time (rtt/rtvar): 0.0ms/250.0ms
    Delayed Ack Timeout (ato): 0.0ms
    Congestion Window (cwnd): 1
    Slow-start Threshold (ssthresh): 7

BGP neighbor is 10.0.0.128, remote AS 64512, internal link
 Description: Huawei_128
  BGP version 4, remote router ID 10.0.0.128, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 3d22h, last write 3d22h
  Hold time is 180, keepalive interval is 60 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is inactive
  Keepalive timer is inactive
  Connect timer is active, time left: 00:00:07
  Connection interval is 20 seconds
  Failed connection attempts is 205
  Idle-restart timer is inactive
  BGP state is Connect
  Number of transitions to established: 1
  Last state was Active
  Last event was ConnectRetry
  Last sent notification:Open Message Error/unsupported capability, Last time 3d22h, First time 3d22h, Repeats 38
    Sent data: 0x010400010080010400020080
  Last rcvd notification:Cease/peer de-configured, Last time 3d22h
  Last sent socket-error:Connect (Network is unreachable), Last time 01:19:37, First time 18:23:30, Repeats 7
  Last rcvd socket-error:Connection reset by peer, Last time 3d22h, First time 3d22h, Repeats 5
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
TCP Socket Information:
  TCP state is SYN-SENT
  Recv-Q: 0/131072
  Send-Q: 0/16384
  Outgoing Maximum Segment Size (MSS): 524
  Total Number of TCP retransmissions: 4
  Options:
    Timestamps enabled: no
    Selective Acknowledgments enabled: no
    Window Scale enabled: no
    Explicit Congestion Notification (ECN) enabled: no
  Socket Statistics:
    Window Scale (wscale): 0,0
    Retransmission Timeout (rto): 16000.0ms
    Round-trip Time (rtt/rtvar): 0.0ms/250.0ms
    Delayed Ack Timeout (ato): 0.0ms
    Congestion Window (cwnd): 1
    Slow-start Threshold (ssthresh): 7

BGP neighbor is 10.0.0.131, remote AS 64512, internal link
 Description: Juniper-131-JCNR
  BGP version 4, remote router ID 10.0.0.131, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 18:25:25, last write 18:23:55
  Hold time is 90, keepalive interval is 30 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is inactive
  Keepalive timer is inactive
  Connect timer is active, time left: 00:00:11
  Connection interval is 20 seconds
  Failed connection attempts is 2847
  Idle-restart timer is inactive
  BGP state is Connect
  Number of transitions to established: 2
  Last state was Active
  Last event was ConnectRetry
  Last sent notification:Hold Timer Expired Error/None, Last time 18:23:55
  Last rcvd notification:Cease/connection rejected, Last time 19:46:37
  Last sent socket-error:Connect (Network is unreachable), Last time 18:07:50, First time 18:21:52, Repeats 8
  Types of communities advertised: standard extended large
  Neighbor is a route reflector client
  Neighbor is using global cluster ID 10.0.0.30
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
    Opens:                  3         3
    Notifications:          1         1
    Updates:              494         8
    Keepalives:         13174     12446
    Route Refresh:          0         0
    Total messages:     13672     12458
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
Remote TCP address is 10.0.0.131, remote port is 179
TCP Socket Information:
  TCP state is SYN-SENT
  Recv-Q: 0/131072
  Send-Q: 0/16384
  Outgoing Maximum Segment Size (MSS): 524
  Total Number of TCP retransmissions: 3
  Options:
    Timestamps enabled: no
    Selective Acknowledgments enabled: no
    Window Scale enabled: no
    Explicit Congestion Notification (ECN) enabled: no
  Socket Statistics:
    Window Scale (wscale): 0,0
    Retransmission Timeout (rto): 8000.0ms
    Round-trip Time (rtt/rtvar): 0.0ms/250.0ms
    Delayed Ack Timeout (ato): 0.0ms
    Congestion Window (cwnd): 1
    Slow-start Threshold (ssthresh): 7

BGP neighbor is 10.0.0.156, remote AS 64512, internal link
 Description: Juniper-156
  BGP version 4, remote router ID 10.0.0.156, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 18:25:45, last write 18:24:15
  Hold time is 90, keepalive interval is 30 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is inactive
  Keepalive timer is inactive
  Connect timer is active, time left: 00:00:36
  Connection interval is 148 seconds
  Failed connection attempts is 394
  Idle-restart timer is inactive
  BGP state is Active
  Number of transitions to established: 4
  Last state was Connect
  Last event was TransportError
  Last sent notification:Hold Timer Expired Error/None, Last time 18:24:15, First time 18:45:09, Repeats 1
  Last rcvd notification:Cease/connection rejected, Last time 19:46:37
  Last sent socket-error:Connect (Network is unreachable), Last time 00:01:58, First time 18:21:58, Repeats 393
  Types of communities advertised: standard extended large
  Neighbor is a route reflector client
  Neighbor is using global cluster ID 10.0.0.30
  Neighbor Capabilities:
    Multiprotocol VPN-IPv4: advertised and received
    Multiprotocol VPN-IPv6: advertised
    Multiprotocol L2VPN EVPN: received
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
    Opens:                  5         5
    Notifications:          2         2
    Updates:              446       105
    Keepalives:         13146     12388
    Route Refresh:          0         0
    Total messages:     13599     12500
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
Remote TCP address is 10.0.0.156, remote port is 179

BGP neighbor is 10.0.0.179, remote AS 64512, internal link
 Description: Juniper-179
  BGP version 4, remote router ID 10.0.0.179, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 18:25:42, last write 18:24:12
  Hold time is 90, keepalive interval is 30 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is inactive
  Keepalive timer is inactive
  Connect timer is active, time left: 00:00:14
  Connection interval is 20 seconds
  Failed connection attempts is 2844
  Idle-restart timer is inactive
  BGP state is Connect
  Number of transitions to established: 3
  Last state was Active
  Last event was ConnectRetry
  Last sent notification:Hold Timer Expired Error/None, Last time 18:24:12, First time 23:21:10, Repeats 1
  Last rcvd notification:Cease/connection rejected, Last time 19:46:37
  Last sent socket-error:Connect (Network is unreachable), Last time 18:07:50, First time 18:22:03, Repeats 8
  Types of communities advertised: standard extended large
  Neighbor is a route reflector client
  Neighbor is using global cluster ID 10.0.0.30
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
    Opens:                338       338
    Notifications:        336         1
    Updates:              501        22
    Keepalives:         10896     10303
    Route Refresh:          0         2
    Total messages:     12071     10666
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
Remote TCP address is 10.0.0.179, remote port is 179
TCP Socket Information:
  TCP state is SYN-SENT
  Recv-Q: 0/131072
  Send-Q: 0/16384
  Outgoing Maximum Segment Size (MSS): 524
  Total Number of TCP retransmissions: 2
  Options:
    Timestamps enabled: no
    Selective Acknowledgments enabled: no
    Window Scale enabled: no
    Explicit Congestion Notification (ECN) enabled: no
  Socket Statistics:
    Window Scale (wscale): 0,0
    Retransmission Timeout (rto): 4000.0ms
    Round-trip Time (rtt/rtvar): 0.0ms/250.0ms
    Delayed Ack Timeout (ato): 0.0ms
    Congestion Window (cwnd): 1
    Slow-start Threshold (ssthresh): 7

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
  Connect timer is active, time left: 00:01:58
  Connection interval is 148 seconds
  Failed connection attempts is 391
  Idle-restart timer is inactive
  BGP state is Active
  Number of transitions to established: 0
  Last state was Connect
  Last event was TransportError
  Last sent socket-error:Connect (Network is unreachable), Last time 00:00:41, First time 4d16h, Repeats 2385
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
  Last read 23:04:12, last write 18:28:03
  Hold time is 90, keepalive interval is 30 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is inactive
  Keepalive timer is inactive
  Connect timer is active, time left: 00:00:14
  Connection interval is 20 seconds
  Failed connection attempts is 14
  Idle-restart timer is inactive
  BGP state is Connect
  Number of transitions to established: 1
  Last state was Active
  Last event was ConnectRetry
  Last rcvd notification:Cease/administrative shutdown, Last time 23:04:12
  Last sent socket-error:Connect (Network is unreachable), Last time 00:04:44, First time 00:36:59, Repeats 2
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
Local TCP address is 10.0.0.30
Remote TCP address is 10.0.0.214, remote port is 179
TCP Socket Information:
  TCP state is SYN-SENT
  Recv-Q: 0/131072
  Send-Q: 0/16384
  Outgoing Maximum Segment Size (MSS): 524
  Total Number of TCP retransmissions: 2
  Options:
    Timestamps enabled: no
    Selective Acknowledgments enabled: no
    Window Scale enabled: no
    Explicit Congestion Notification (ECN) enabled: no
  Socket Statistics:
    Window Scale (wscale): 0,0
    Retransmission Timeout (rto): 4000.0ms
    Round-trip Time (rtt/rtvar): 0.0ms/250.0ms
    Delayed Ack Timeout (ato): 0.0ms
    Congestion Window (cwnd): 1
    Slow-start Threshold (ssthresh): 7

BGP neighbor is 10.0.0.216, remote AS 64512, internal link
 Description: 2-23-5G-NOKIA-216
  BGP version 4, remote router ID 10.0.0.216, VRF default
  Inherits configuration from and member of peer-group 2-23-5G-RR
  Last read 00:00:07, last write 00:00:10
  Hold time is 90, keepalive interval is 30 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:01:23
  Keepalive timer is active, time left: 00:00:15
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 17:09:10
  Number of transitions to established: 4
  Last state was OpenConfirm
  Last event was RecvRtRefresh
  Last sent notification:Cease/other configuration change, Last time 18:07:44
  Last rcvd notification:Cease/administrative reset, Last time 17:09:10
  Types of communities advertised: standard extended large
  Neighbor Capabilities:
    Multiprotocol VPN-IPv4: advertised and received and negotiated
    Multiprotocol L2VPN EVPN: advertised and received and negotiated
    Four Octet ASN: advertised and received and negotiated
    Route Refresh: advertised and received and negotiated
    Enhanced route refresh: advertised
    Send End-of-RIB messages: advertised and received and negotiated
    Additional-paths recv capability:
      VPN-IPv4: negotiated
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
    VPN-IPv4 End-of-RIB received: Yes
      Received 17:09:10
      Number of stale paths removed after graceful restart: 0
      Number of paths received before End-of-RIB: 4
    L2VPN EVPN End-of-RIB received: Yes
      Received 17:09:10
      Number of stale paths removed after graceful restart: 0
      Number of paths received before End-of-RIB: 18
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
    Notifications:          1         2
    Updates:               52      1619
    Keepalives:          2565      2193
    Route Refresh:          0         8
    Total messages:      2622      3826
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    VPN-IPv4:                         2        15             15                  11
    IPv6 Unicast:                     0         0              0                   0
    EVPN:                             3        51             37                  29
  Configured maximum total number of routes is 256000, warning limit is 204800
  Inbound updates dropped by reason:
    AS path loop detection: 0
    Cluster ID loop detection: 0
    Enforced First AS: 0
    Malformed MPBGP routes: 19
    Originator ID matches local router ID: 0
    Nexthop matches local IP address: 8
    Unexpected IPv6 nexthop for IPv4 routes: 0
    AS_SET/AS_CONFED_SET in AS_PATH for IPv4 Unicast: 0
    AS_SET/AS_CONFED_SET in AS_PATH for IPv6 Unicast: 0
  Inbound updates with attribute errors:
    Resulting in removal of all paths in update (treat as withdraw): 8
    Resulting in AFI/SAFI disable: 0
    Resulting in attribute ignore: 0
    Disabled AFI/SAFIs: None
    Last treat-as-withdraw attribute error: Nexthop is local address
    Last update with error received at: 14:51:31
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
    L2VPN EVPN NLRIs dropped due to maximum route limit violation: 0
    Link-state NLRIs dropped because reception is unsupported: 0
    RT Membership NLRIs dropped due to local origin ASN received from external peer: 0
  Outbound paths dropped by reason:
    IPv4 local address not available: 0
    IPv6 local address not available: 0
Local AS is 64512, local router ID 10.0.0.30
TTL is 255
Local TCP address is 10.0.30.30, local port is 179
Remote TCP address is 10.0.0.216, remote port is 50728
Local next hop for next hop self:
  VPN-IPv4: 10.0.30.30
  L2VPN EVPN: 10.0.30.30
TCP Socket Information:
  TCP state is ESTABLISHED
  Recv-Q: 0/32768
  Send-Q: 0/46080
  Outgoing Maximum Segment Size (MSS): 1012
  Total Number of TCP retransmissions: 5
  Options:
    Timestamps enabled: yes
    Selective Acknowledgments enabled: no
    Window Scale enabled: yes
    Explicit Congestion Notification (ECN) enabled: no
  Socket Statistics:
    Window Scale (wscale): 0,7
    Retransmission Timeout (rto): 256.0ms
    Round-trip Time (rtt/rtvar): 23.3ms/39.9ms
    Delayed Ack Timeout (ato): 40.0ms
    Congestion Window (cwnd): 2
    Slow-start Threshold (ssthresh): 2
    TCP Throughput: 0.70 Mbps
    Recv Round-trip Time (rcv_rtt): 1.0ms
    Advertised Recv Window (rcv_space): 14600

BGP neighbor is 10.0.0.217, remote AS 64512, internal link
 Description: Nokia
  BGP version 4, remote router ID 10.0.0.217, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 18:25:36, last write 18:24:06
  Hold time is 90, keepalive interval is 30 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is inactive
  Keepalive timer is inactive
  Connect timer is active, time left: 00:00:04
  Connection interval is 20 seconds
  Failed connection attempts is 1869
  Idle-restart timer is inactive
  BGP state is Connect
  Number of transitions to established: 2
  Last state was Active
  Last event was ConnectRetry
  Last sent notification:Hold Timer Expired Error/None, Last time 18:24:06
  Last sent socket-error:Connect (Network is unreachable), Last time 11:55:57, First time 18:21:57, Repeats 10
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
Local TCP address is 10.0.0.30
Remote TCP address is 10.0.0.217, remote port is 179
TCP Socket Information:
  TCP state is SYN-SENT
  Recv-Q: 0/131072
  Send-Q: 0/16384
  Outgoing Maximum Segment Size (MSS): 524
  Total Number of TCP retransmissions: 4
  Options:
    Timestamps enabled: no
    Selective Acknowledgments enabled: no
    Window Scale enabled: no
    Explicit Congestion Notification (ECN) enabled: no
  Socket Statistics:
    Window Scale (wscale): 0,0
    Retransmission Timeout (rto): 16000.0ms
    Round-trip Time (rtt/rtvar): 0.0ms/250.0ms
    Delayed Ack Timeout (ato): 0.0ms
    Congestion Window (cwnd): 1
    Slow-start Threshold (ssthresh): 7

BGP neighbor is 10.0.0.221, remote AS 64512, internal link
 Description: Ribbon-221
  BGP version 4, remote router ID 10.0.0.221, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 18:25:45, last write 18:22:45
  Hold time is 180, keepalive interval is 60 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is inactive
  Keepalive timer is inactive
  Connect timer is active, time left: 00:00:07
  Connection interval is 20 seconds
  Failed connection attempts is 62
  Idle-restart timer is inactive
  BGP state is Connect
  Number of transitions to established: 15
  Last state was Active
  Last event was ConnectRetry
  Last sent notification:Hold Timer Expired Error/None, Last time 18:22:45, First time 3d23h, Repeats 5
  Last sent socket-error:Connect (Network is unreachable), Last time 00:25:19, First time 3d16h, Repeats 50
  Last rcvd socket-error:Connection reset by peer, Last time 18:36:26, First time 4d16h, Repeats 8
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
    Opens:                 16        15
    Notifications:          6         0
    Updates:              922        48
    Keepalives:          6497     15240
    Route Refresh:         20        10
    Total messages:      7461     15313
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
Remote TCP address is 10.0.0.221, remote port is 179
TCP Socket Information:
  TCP state is SYN-SENT
  Recv-Q: 0/131072
  Send-Q: 0/16384
  Outgoing Maximum Segment Size (MSS): 524
  Total Number of TCP retransmissions: 3
  Options:
    Timestamps enabled: no
    Selective Acknowledgments enabled: no
    Window Scale enabled: no
    Explicit Congestion Notification (ECN) enabled: no
  Socket Statistics:
    Window Scale (wscale): 0,0
    Retransmission Timeout (rto): 8000.0ms
    Round-trip Time (rtt/rtvar): 0.0ms/250.0ms
    Delayed Ack Timeout (ato): 0.0ms
    Congestion Window (cwnd): 1
    Slow-start Threshold (ssthresh): 7

BGP neighbor is 10.0.1.156, remote AS 64512, internal link
 Description: 2-23-5G-JUNIPER-156
  BGP version 4, remote router ID 10.0.0.156, VRF default
  Inherits configuration from and member of peer-group 2-23-5G-RR
  Last read 00:00:11, last write 00:00:23
  Hold time is 90, keepalive interval is 30 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:01:19
  Keepalive timer is inactive
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 17:18:55
  Number of transitions to established: 3
  Last state was OpenConfirm
  Last event was RecvUpdate
  Last sent notification:Cease/other configuration change, Last time 18:07:44
  Last rcvd notification:Cease/peer de-configured, Last time 17:18:56
  Types of communities advertised: standard extended large
  Neighbor Capabilities:
    Multiprotocol VPN-IPv4: advertised and received and negotiated
    Multiprotocol L2VPN EVPN: advertised and received and negotiated
    Four Octet ASN: advertised and received and negotiated
    Route Refresh: advertised and received and negotiated
    Enhanced route refresh: advertised
    Send End-of-RIB messages: advertised and received and negotiated
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
    VPN-IPv4 End-of-RIB received: Yes
      Received 17:18:55
      Number of stale paths removed after graceful restart: 0
      Number of paths received before End-of-RIB: 4
    L2VPN EVPN End-of-RIB received: Yes
      Received 17:18:55
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
    Opens:                  3         3
    Notifications:          1         1
    Updates:               23       232
    Keepalives:          2569      2352
    Route Refresh:          0         0
    Total messages:      2596      2588
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    VPN-IPv4:                         2        15             15                   0
    IPv6 Unicast:                     0         0              0                   0
    EVPN:                             3        29             29                   0
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
    L2VPN EVPN NLRIs dropped due to maximum route limit violation: 0
    Link-state NLRIs dropped because reception is unsupported: 0
    RT Membership NLRIs dropped due to local origin ASN received from external peer: 0
  Outbound paths dropped by reason:
    IPv4 local address not available: 0
    IPv6 local address not available: 0
Local AS is 64512, local router ID 10.0.0.30
TTL is 255
Local TCP address is 10.0.30.30, local port is 35073
Remote TCP address is 10.0.1.156, remote port is 179
Local next hop for next hop self:
  VPN-IPv4: 10.0.30.30
  L2VPN EVPN: 10.0.30.30
TCP Socket Information:
  TCP state is ESTABLISHED
  Recv-Q: 0/32768
  Send-Q: 0/46080
  Outgoing Maximum Segment Size (MSS): 1448
  Total Number of TCP retransmissions: 8
  Options:
    Timestamps enabled: yes
    Selective Acknowledgments enabled: yes
    Window Scale enabled: yes
    Explicit Congestion Notification (ECN) enabled: no
  Socket Statistics:
    Window Scale (wscale): 0,7
    Retransmission Timeout (rto): 204.0ms
    Round-trip Time (rtt/rtvar): 0.7ms/0.6ms
    Delayed Ack Timeout (ato): 40.0ms
    Congestion Window (cwnd): 3
    Slow-start Threshold (ssthresh): 7
    TCP Throughput: 51.11 Mbps
    Recv Round-trip Time (rcv_rtt): 3494.0ms
    Advertised Recv Window (rcv_space): 14480

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
10.0.0.54/32    IS-IS SR IPv4   29          65                  115            
10.0.0.66/32    IS-IS SR IPv4   13          65                  115            
10.0.0.72/32    IS-IS SR IPv4   14          65                  115            
10.0.0.84/32    IS-IS SR IPv4   8           65                  115            
10.0.0.120/32   IS-IS SR IPv4   17          65                  115            
10.0.0.124/32   IS-IS SR IPv4   22          65                  115            
10.0.0.128/32   IS-IS SR IPv4   18          65                  115            
10.0.0.131/32   IS-IS SR IPv4   9           65                  115            
10.0.0.175/32   IS-IS SR IPv4   7           65                  115            
10.0.0.179/32   IS-IS SR IPv4   12          65                  115            
10.0.0.185/32   IS-IS SR IPv4   28          65                  115            
10.0.0.214/32   IS-IS SR IPv4   21          65                  115            
10.0.0.216/32   IS-IS SR IPv4   25          65                  115            
10.0.0.217/32   IS-IS SR IPv4   16          65                  115            
10.0.0.221/32   IS-IS SR IPv4   15          65                  115            
10.0.1.156/32   IS-IS SR IPv4   24          65                  115            
10.0.1.179/32   IS-IS SR IPv4   23          65                  115            

   IGP Metric    Metric Type
---------------- -----------
   32            metric     
   11            metric     
   21            metric     
   11            metric     
   31            metric     
   21            metric     
   21            metric     
   21            metric     
   21            metric     
   32            metric     
   22            metric     
   23            metric     
   31            metric     
   11            metric     
   21            metric     
   32            metric     
   32            metric     
   11            metric     
   11            metric     

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
>C    10.0.0.30/32 [0 pref/0 metric] updated 19:46:39 ago
         via Loopback0, directly connected
>C    10.0.30.30/32 [0 pref/0 metric] updated 19:46:07 ago
         via Loopback1000, directly connected
>C    20.30.66.0/24 [0 pref/0 metric] updated 3d15h ago
         via Ethernet31, directly connected
>C    20.30.184.0/24 [0 pref/0 metric] updated 4d18h ago
         via Ethernet7, directly connected
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
>P    0.0.0.0/8 [1 pref/0 metric] updated 4d18h ago
         via Null0, directly connected [NF]
>P    127.0.0.0/8 [1 pref/0 metric] updated 4d18h ago
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
>I    10.0.0.32/32 [115 pref/32 metric] updated 18:07:51 ago
         via 20.30.66.66, Ethernet31
>I    10.0.0.53/32 [115 pref/11 metric] updated 18:23:32 ago
         via 20.30.66.66, Ethernet31
>I    10.0.0.54/32 [115 pref/21 metric] updated 18:06:40 ago
         via 20.30.66.66, Ethernet31
>I    10.0.0.66/32 [115 pref/11 metric] updated 18:23:32 ago
         via 20.30.66.66, Ethernet31
>I    10.0.0.72/32 [115 pref/31 metric] updated 18:03:51 ago
         via 20.30.66.66, Ethernet31
>I    10.0.0.84/32 [115 pref/21 metric] updated 18:23:32 ago
         via 20.30.66.66, Ethernet31
>I    10.0.0.120/32 [115 pref/21 metric] updated 18:07:51 ago
         via 20.30.66.66, Ethernet31
>I    10.0.0.124/32 [115 pref/21 metric] updated 01:18:28 ago
         via 20.30.66.66, Ethernet31
>I    10.0.0.128/32 [115 pref/21 metric] updated 01:18:35 ago
         via 20.30.66.66, Ethernet31
>I    10.0.0.131/32 [115 pref/32 metric] updated 18:07:51 ago
         via 20.30.66.66, Ethernet31
>I    10.0.0.175/32 [115 pref/22 metric] updated 18:07:51 ago
         via 20.30.66.66, Ethernet31
>I    10.0.0.179/32 [115 pref/23 metric] updated 18:07:51 ago
         via 20.30.66.66, Ethernet31
>I    10.0.0.185/32 [115 pref/31 metric] updated 01:26:04 ago
         via 20.30.66.66, Ethernet31
>I    10.0.0.214/32 [115 pref/11 metric] updated 00:04:46 ago
         via 20.30.66.66, Ethernet31
>I    10.0.0.216/32 [115 pref/21 metric] updated 18:23:31 ago
         via 20.30.66.66, Ethernet31
>I    10.0.0.217/32 [115 pref/32 metric] updated 11:53:54 ago
         via 20.30.66.66, Ethernet31
>I    10.0.0.221/32 [115 pref/32 metric] updated 00:23:45 ago
         via 20.30.66.66, Ethernet31
>I    10.0.1.156/32 [115 pref/11 metric] updated 17:04:33 ago
         via 20.30.66.66, Ethernet31
>I    10.0.1.179/32 [115 pref/11 metric] updated 18:23:31 ago
         via 20.30.66.66, Ethernet31
>I    20.32.175.0/24 [115 pref/32 metric] updated 18:07:51 ago
         via 20.30.66.66, Ethernet31
>I    20.53.66.0/24 [115 pref/11 metric] updated 18:23:32 ago
         via 20.30.66.66, Ethernet31
>I    20.53.72.0/24 [115 pref/21 metric] updated 18:03:58 ago
         via 20.30.66.66, Ethernet31
>I    20.53.120.0/24 [115 pref/21 metric] updated 18:15:00 ago
         via 20.30.66.66, Ethernet31
>I    20.53.124.0/24 [115 pref/21 metric] updated 01:18:36 ago
         via 20.30.66.66, Ethernet31
>I    20.53.128.0/24 [115 pref/21 metric] updated 01:18:36 ago
         via 20.30.66.66, Ethernet31
>I    20.53.185.0/24 [115 pref/21 metric] updated 18:23:32 ago
         via 20.30.66.66, Ethernet31
>I    20.53.216.0/24 [115 pref/21 metric] updated 18:23:32 ago
         via 20.30.66.66, Ethernet31
>I    20.54.66.0/24 [115 pref/11 metric] updated 18:23:32 ago
         via 20.30.66.66, Ethernet31
>I    20.66.84.0/24 [115 pref/11 metric] updated 18:23:32 ago
         via 20.30.66.66, Ethernet31
>I    20.66.156.0/24 [115 pref/11 metric] updated 17:04:34 ago
         via 20.30.66.66, Ethernet31
>I    20.66.175.0/24 [115 pref/32 metric] updated 18:07:51 ago
         via 20.30.66.66, Ethernet31
>I    20.66.179.0/24 [115 pref/11 metric] updated 18:23:32 ago
         via 20.30.66.66, Ethernet31
>I    20.66.214.0/24 [115 pref/11 metric] updated 18:23:32 ago
         via 20.30.66.66, Ethernet31
>I    20.72.175.0/24 [115 pref/32 metric] updated 18:07:51 ago
         via 20.30.66.66, Ethernet31
>I    20.120.175.0/24 [115 pref/22 metric] updated 18:07:51 ago
         via 20.30.66.66, Ethernet31
>I    20.120.214.0/24 [115 pref/31 metric] updated 18:07:51 ago
         via 20.30.66.66, Ethernet31
>I    20.120.217.0/24 [115 pref/21 metric] updated 11:54:02 ago
         via 20.30.66.66, Ethernet31
>I    20.128.175.0/24 [115 pref/32 metric] updated 01:18:36 ago
         via 20.30.66.66, Ethernet31
>I    20.131.175.0/24 [115 pref/32 metric] updated 18:07:51 ago
         via 20.30.66.66, Ethernet31
>I    20.156.216.0/24 [115 pref/31 metric] updated 15:14:45 ago
         via 20.30.66.66, Ethernet31
>I    20.175.179.0/24 [115 pref/23 metric] updated 18:07:51 ago
         via 20.30.66.66, Ethernet31
>I    20.175.184.0/24 [115 pref/32 metric] updated 18:07:51 ago
         via 20.30.66.66, Ethernet31
>I    20.175.214.0/24 [115 pref/32 metric] updated 18:07:51 ago
         via 20.30.66.66, Ethernet31
>I    20.175.217.0/24 [115 pref/32 metric] updated 11:54:03 ago
         via 20.30.66.66, Ethernet31
>I    20.175.221.0/24 [115 pref/32 metric] updated 00:24:37 ago
         via 20.30.66.66, Ethernet31
>I    21.120.175.0/24 [115 pref/23 metric] updated 18:07:51 ago
         via 20.30.66.66, Ethernet31
>I    21.175.179.0/24 [115 pref/23 metric] updated 18:07:51 ago
         via 20.30.66.66, Ethernet31
>I    192.168.20.0/23 [115 pref/21 metric] updated 18:07:51 ago
         via 20.30.66.66, Ethernet31
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
>C    2001:0:30:66::/64 [0 pref/0 metric] updated 3d15h ago
         via Ethernet31, directly connected
>C    2001:0:30:184::/64 [0 pref/0 metric] updated 4d18h ago
         via Ethernet7, directly connected
>C    2002::30/128 [0 pref/0 metric] updated 19:46:39 ago
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
>P    ::/96 [1 pref/0 metric] updated 4d18h ago
         via Null0, directly connected [NF]
>P    ::ffff:127.0.0.0/104 [1 pref/0 metric] updated 4d18h ago
         via :: [1 pref/1 metric] type ipv6
            via , directly connected
>P    fe80::/10 [1 pref/0 metric] updated 4d18h ago
```

## show platform sand l3 summary

```text
Number of vrfs: 5

Ipv4:
  Routes:       103  backlog:  0  unprogrammed:  0
  Adjacencies:  76   backlog:  0  unprogrammed:  0
Ipv6:
  Routes:       13  backlog:  0  unprogrammed:  0
  Adjacencies:  76  backlog:  0  unprogrammed:  0
Mpls:
  Routes:       20  backlog:  0  unprogrammed:  0
  Adjacencies:  1   backlog:  0  unprogrammed:  0

Jericho2 Ip Fecs:
  Non-ecmp fecs:  4133  ecmp fecs:  0  fec entries:  4133
Jericho2 Mpls Fecs:
  Non-ecmp fecs:  1  ecmp fecs:  0  fec entries:  1
Jericho2 Vxlan Tunnel Fecs:
  Non-ecmp fecs:  0  ecmp fecs:  0  fec entries:  0
  Number of vxlan tunnels configured: 0

Jericho2 Lpm Routes:
  Routes:   103  unprogrammed:   0   
  Routes6:  13   unprogrammed6:  0   
  Backlog:  0  

Jericho2 Lpm:
  TCAM entries used:   4   Percent free:  99  ADS2 entries used:   7  Percent free:  99
  Pivot buckets used:  6   Rows used:     2   Entries Per Bucket:  1  Percent free:  99
  Route buckets used:  20  Rows used:     3   Entries Per Bucket:  5  Percent free:  99

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
  FixedSystem: 0
Egress Mpls (for inner 2 labels) rewrite entries in use (in each fap):
  FixedSystem: 18
Egress Sflow rewrite entries in use (in each fap):
  FixedSystem: 0

Egress rewrite chains in backlog: resource-full 0, no-interface 0

Glem entries used per fap :
  FixedSystem: 4116

Jericho2 Fec:
  Maximum FEC hierarchy levels:  2
  ReusedEcmp:  793  allocs:  5063  frees:  5028  shuffles:  0  cmds:  0
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
    Non-ecmp fecs:            40  ecmp fecs:            0  
    Non-ecmp (Percent free):  99  ecmp (Percent free):  100
  Level3  Fecs:
    Non-ecmp fecs:            30  ecmp fecs:            0  
    Non-ecmp (Percent free):  99  ecmp (Percent free):  100

Lpm Detail:
  Requests:  9212  cleanses:  1481  batches:  1481  avg batch size:  6

Jericho Arp:
  ArpTable writes:      131132  queued      0   
  IngressTable writes:  167542  queued      0   
  Coprocessors:         1       in CmdRing

Tunnel Counter Status
  Number of MPLS tunnels:                  18   
  Number of uncountable MPLS tunnels:      18   
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
|0  |10.0.0.32/32      |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318768|   -   
|0  |10.0.0.53/32      |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318768|   -   
|0  |10.0.0.54/32      |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318768|   -   
|0  |10.0.0.66/32      |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318768|   -   
|0  |10.0.0.72/32      |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318768|   -   
|0  |10.0.0.84/32      |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318768|   -   
|0  |10.0.0.120/32     |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318768|   -   
|0  |10.0.0.124/32     |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318768|   -   
|0  |10.0.0.128/32     |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318768|   -   
|0  |10.0.0.131/32     |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318768|   -   
|0  |10.0.0.175/32     |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318768|   -   
|0  |10.0.0.179/32     |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318768|   -   
|0  |10.0.0.185/32     |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318768|   -   
|0  |10.0.0.214/32     |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318768|   -   
|0  |10.0.0.216/32     |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318768|   -   
|0  |10.0.0.217/32     |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318768|   -   
|0  |10.0.0.221/32     |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318768|   -   
|0  |10.0.1.156/32     |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318768|   -   
|0  |10.0.1.179/32     |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318768|   -   
|0  |10.0.30.30/32     |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.66.0/32     |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.66.30/32    |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.66.66/32    |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318992|   -   
|0  |20.30.66.255/32   |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.66.0/24     |TRAP | CoppSystemL3DstMiss|1020 |1020    | ArpTrap           |  -  |315691|   -   
|0  |20.30.184.0/32    |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.184.30/32   |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.184.255/32  |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.184.0/24    |TRAP | CoppSystemL3DstMiss|1010 |1010    | ArpTrap           |  -  |315681|   -   
|0  |20.32.175.0/24    |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318768|   -   
|0  |20.53.66.0/24     |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318768|   -   
|0  |20.53.72.0/24     |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318768|   -   
|0  |20.53.120.0/24    |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318768|   -   
|0  |20.53.124.0/24    |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318768|   -   
|0  |20.53.128.0/24    |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318768|   -   
|0  |20.53.185.0/24    |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318768|   -   
|0  |20.53.216.0/24    |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318768|   -   
|0  |20.54.66.0/24     |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318768|   -   
|0  |20.66.84.0/24     |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318768|   -   
|0  |20.66.156.0/24    |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318768|   -   
|0  |20.66.175.0/24    |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318768|   -   
|0  |20.66.179.0/24    |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318768|   -   
|0  |20.66.214.0/24    |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318768|   -   
|0  |20.72.175.0/24    |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318768|   -   
|0  |20.120.175.0/24   |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318768|   -   
|0  |20.120.214.0/24   |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318768|   -   
|0  |20.120.217.0/24   |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318768|   -   
|0  |20.128.175.0/24   |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318768|   -   
|0  |20.131.175.0/24   |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318768|   -   
|0  |20.156.216.0/24   |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318768|   -   
|0  |20.175.179.0/24   |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318768|   -   
|0  |20.175.184.0/24   |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318768|   -   
|0  |20.175.214.0/24   |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318768|   -   
|0  |20.175.217.0/24   |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318768|   -   
|0  |20.175.221.0/24   |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318768|   -   
|0  |21.120.175.0/24   |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318768|   -   
|0  |21.175.179.0/24   |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318768|   -   
|0  |127.0.0.0/8       |TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |  -  |314671|   -   
|0  |192.168.20.0/23   |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318768|   -   
|0  |0.0.0.0/0         |TRAP | CoppSystemL3LpmOver|0    |  -     | SlowReceive       |  -  |314669|   -   
|1  |0.0.0.0/8         |DROP | DROP               |0    |  -     |                   |  -  |318968|   -   
|1  |10.0.0.30/32      |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|1  |50.10.120.0/24    |ROUTE| FEC 318958         |0    |2097146 | 00:00:00:00:00:00 |  -  |183520|M 20120 1275
|1  |50.10.156.0/24    |ROUTE| FEC 318958         |0    |2097149 | 00:00:00:00:00:00 |  -  |183508|M 20456 16
|1  |50.10.179.0/24    |ROUTE| FEC 318958         |0    |2097150 | 00:00:00:00:00:00 |  -  |183504|M 20479 16
|1  |127.0.0.0/8       |TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |  -  |314671|   -   
|1  |0.0.0.0/0         |TRAP | CoppSystemL3LpmOver|0    |  -     | SlowReceive       |  -  |314669|   -   
|2  |0.0.0.0/8         |DROP | DROP               |0    |  -     |                   |  -  |318970|   -   
|2  |10.128.0.30/32    |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|2  |50.128.120.0/24   |ROUTE| FEC 318958         |0    |2097147 | 00:00:00:00:00:00 |  -  |183518|M 20120 1278
|2  |50.128.156.0/24   |ROUTE| FEC 318958         |0    |2097148 | 00:00:00:00:00:00 |  -  |183512|M 20456 17
|2  |50.129.120.0/24   |ROUTE| FEC 318958         |0    |2097145 | 00:00:00:00:00:00 |  -  |183522|M 20120 1277
|2  |50.129.156.0/24   |ROUTE| FEC 318958         |0    |2097148 | 00:00:00:00:00:00 |  -  |183510|M 20456 17
|2  |50.130.120.0/24   |ROUTE| FEC 318958         |0    |2097144 | 00:00:00:00:00:00 |  -  |183524|M 20120 1276
|2  |50.130.156.0/24   |ROUTE| FEC 318958         |0    |2097148 | 00:00:00:00:00:00 |  -  |183514|M 20456 17
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
|4  |50.10.30.0/32     |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|4  |50.10.30.1/32     |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|4  |50.10.30.2/32     |ROUTE| Et46/1             |1008 |103421  | 00:14:01:00:00:01 |  -  |318962|   -   
|4  |50.10.30.255/32   |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|4  |50.10.30.0/24     |TRAP | CoppSystemL3DstMiss|1008 |1008    | ArpTrap           |  -  |315679|   -   
|4  |50.10.54.0/24     |ROUTE| FEC 318958         |0    |2097135 | 00:00:00:00:00:00 |  -  |183538|M 20054 970000
|4  |50.10.72.0/24     |ROUTE| FEC 318958         |0    |2097139 | 00:00:00:00:00:00 |  -  |183534|M 20072 62000
|4  |50.10.84.0/24     |ROUTE| FEC 318958         |0    |2097133 | 00:00:00:00:00:00 |  -  |183506|M 20084 720897
|4  |50.10.120.0/24    |ROUTE| FEC 318958         |0    |2097140 | 00:00:00:00:00:00 |  -  |183532|M 20120 1274
|4  |50.10.124.0/24    |ROUTE| FEC 318958         |0    |2097138 | 00:00:00:00:00:00 |  -  |183528|M 20124 303
|4  |50.10.179.0/24    |ROUTE| FEC 318958         |0    |2097141 | 00:00:00:00:00:00 |  -  |183530|M 20479 30
|4  |50.10.185.0/24    |ROUTE| FEC 318958         |0    |2097136 | 00:00:00:00:00:00 |  -  |183502|M 20185 16
|4  |50.10.214.0/24    |ROUTE| FEC 318958         |0    |2097143 | 00:00:00:00:00:00 |  -  |183516|M 20214 500001
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
|  -  |183502|ROUTE| FEC 318958         |   - |2097136 |                 - |Mpush 20185 16
|  -  |183504|ROUTE| FEC 318958         |   - |2097150 |                 - |Mpush 20479 16
|  -  |183506|ROUTE| FEC 318958         |   - |2097133 |                 - |Mpush 20084 720897
|  -  |183508|ROUTE| FEC 318958         |   - |2097149 |                 - |Mpush 20456 16
|  -  |183510|ROUTE| FEC 318958         |   - |2097148 |                 - |Mpush 20456 17
|  -  |183512|ROUTE| FEC 318958         |   - |2097148 |                 - |Mpush 20456 17
|  -  |183514|ROUTE| FEC 318958         |   - |2097148 |                 - |Mpush 20456 17
|  -  |183516|ROUTE| FEC 318958         |   - |2097143 |                 - |Mpush 20214 500001
|  -  |183518|ROUTE| FEC 318958         |   - |2097147 |                 - |Mpush 20120 1278
|  -  |183520|ROUTE| FEC 318958         |   - |2097146 |                 - |Mpush 20120 1275
|  -  |183522|ROUTE| FEC 318958         |   - |2097145 |                 - |Mpush 20120 1277
|  -  |183524|ROUTE| FEC 318958         |   - |2097144 |                 - |Mpush 20120 1276
|  -  |183528|ROUTE| FEC 318958         |   - |2097138 |                 - |Mpush 20124 303
|  -  |183530|ROUTE| FEC 318958         |   - |2097141 |                 - |Mpush 20479 30
|  -  |183532|ROUTE| FEC 318958         |   - |2097140 |                 - |Mpush 20120 1274
|  -  |183534|ROUTE| FEC 318958         |   - |2097139 |                 - |Mpush 20072 62000
|  -  |183538|ROUTE| FEC 318958         |   - |2097135 |                 - |Mpush 20054 970000
|  -  |314666|TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |   -   
|  -  |314667|TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |   -   
|  -  |314669|TRAP | CoppSystemL3LpmOver|0    |  -     | SlowReceive       |   -   
|  -  |314671|TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |   -   
|  -  |315679|TRAP | CoppSystemL3DstMiss|1008 |1008    | ArpTrap           |   -   
|  -  |315681|TRAP | CoppSystemL3DstMiss|1010 |1010    | ArpTrap           |   -   
|  -  |315691|TRAP | CoppSystemL3DstMiss|1020 |1020    | ArpTrap           |   -   
|  -  |318768|ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |   -   
|  -  |318770|ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |   -   
|  -  |318772|DROP | DROP               |0    |  -     |                   |   -   
|  -  |318922|DROP | DROP               |0    |  -     |                   |   -   
|  -  |318956|DROP | DROP               |0    |  -     |                   |   -   
|  -  |318958|ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |   -   
|  -  |318960|DROP | DROP               |0    |  -     |                   |   -   
|  -  |318962|ROUTE| Et46/1             |1008 |103421  | 00:14:01:00:00:01 |   -   
|  -  |318966|DROP | DROP               |0    |  -     |                   |   -   
|  -  |318968|DROP | DROP               |0    |  -     |                   |   -   
|  -  |318970|DROP | DROP               |0    |  -     |                   |   -   
|  -  |318992|ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |   -   

```

