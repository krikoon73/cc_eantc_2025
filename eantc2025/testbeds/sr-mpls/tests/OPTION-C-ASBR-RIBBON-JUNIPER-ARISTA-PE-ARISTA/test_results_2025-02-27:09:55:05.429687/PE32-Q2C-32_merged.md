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

Uptime: 1 week, 3 days, 3 hours and 1 minute
Total memory: 65734472 kB
Free memory: 61716436 kB

```

## show interfaces counters rates | nz

```text
Port      Name                 Intvl  In Mbps      %  In Kpps Out Mbps      %
Et1       Arista_Spine30_Eth2   0:00      4.2   0.0%        5      4.0   0.0%
Et5       Juniper-175_509       0:00      4.2   0.0%        5      4.2   0.0%

Port      Out Kpps
Et1              4
Et5              5
```

## show ip interface brief | exclude una

```text
                                                                        Address
Interface       IP Address          Status      Protocol           MTU  Owner  
--------------- ------------------- ----------- --------------- ------- -------
Ethernet1       20.30.32.32/24      up          up                1500         
Ethernet2       21.30.32.32/24      admin down  down              1500         
Ethernet5       20.32.175.32/24     up          up                1500         
Ethernet40.4    50.10.32.1/24       down        lowerlayerdown    1500         
Ethernet40.128  50.128.32.1/24      down        lowerlayerdown    1500         
Ethernet40.129  50.129.32.1/24      down        lowerlayerdown    1500         
Ethernet40.130  50.130.32.1/24      down        lowerlayerdown    1500         
Loopback0       10.0.0.32/32        up          up               65535         
Loopback201     209.209.209.201/32  up          up               65535         
Loopback202     209.209.209.202/32  up          up               65535         
Management1     192.168.20.32/23    up          up                1500         

```

## show isis neighbors

```text
 
Instance  VRF      System Id        Type Interface          SNPA              State Hold time   Circuit Id          
LEFT      default  Juniper-175-ACX7100-48L L2   Ethernet5          P2P               UP    22          01                  
 
Instance  VRF      System Id        Type Interface          SNPA              State Hold time   Circuit Id          
RIGHT     default  Arista-Spine3-Q2A-30 L2   Ethernet1          P2P               UP    26          79                  
```

## show isis database detail

```text
Legend:
H - hostname conflict
U - node unreachable

IS-IS Instance: LEFT VRF: default
  IS-IS Level 2 Link State Database
    LSPID                   Seq Num  Cksum  Life Length IS  Received LSPID        Flags
    Arista-PE32-Q2C-32.00-00      1147  40403  1065    444 L2  0000.0000.0032.00-00  <>
      LSP generation remaining wait time: 0 ms
      Time remaining until refresh: 765 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Arista-PE32-Q2C-32
      Area addresses: 49.0001
      Topology: 2 (IPv6)
      Topology: 0 (IPv4)
      Interface address: 209.209.209.201
      Interface address: 20.32.175.32
      Interface address: 10.0.0.32
      Interface address: 2001:0:32:175::32
      Interface address: 2002::32
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.32.175.175
        IPv4 Interface Address: 20.32.175.32
        Adj-sid: 362146 flags: [L V] weight: 0x0
      IS Neighbor (MT-IPv6): Juniper-175-ACX7100-48L.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:32:175::175
        Global IPv6 Interface Address: 2001:0:32:175::32
        Adj-sid: 362147 flags: [L V F] weight: 0x0
      Reachability         : 10.0.0.30/32 Metric: 10 Type: 1 Down
        SR Prefix-SID: 30 Flags: [R N P] Algorithm: 0
      Reachability         : 209.209.209.201/32 Metric: 10 Type: 1 Up
        SR Prefix-SID: 201 Flags: [P] Algorithm: 0
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
    Arrcus-53.00-00            2274  29619   883    480 L2  0000.0000.0053.00-00  <>
      Remaining lifetime received: 1197 s Modified to: 1200 s
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
      Reachability         : 20.53.66.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.53.72.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.53.120.0/24 Metric: 10 Type: 1 Up
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
    Ciena-8140-66.00-00          22  46217  1107    227 L2  0000.0000.0066.00-00  <>
      Remaining lifetime received: 1197 s Modified to: 1200 s
      NLPID: 0xCC(IPv4)
      Hostname: Ciena-8140-66
      Area addresses: 49.0001
      Topology: 0 (IPv4)
      Interface address: 20.66.175.66
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.66.175.175
        IPv4 Interface Address: 20.66.175.66
        Adj-sid: 16022 flags: [L V] weight: 0x0
      Reachability         : 20.66.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 10.0.0.66/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 66 Flags: [N] Algorithm: 0
      Reachability         : 209.209.209.201/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 201 Flags: [] Algorithm: 0
      Router Capabilities: Router Id: 10.0.0.66 Flags: []
        SR Capability: Flags: [I]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0
    0000.0000.0120.00-00        503  41223  1090    372 L2  0000.0000.0120.00-00  <>
      Remaining lifetime received: 1197 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Area addresses: 49.0000
      Interface address: 10.0.0.120
      Interface address: 20.120.175.120
      Interface address: 209.209.209.201
      Interface address: 2001:0:120:175::120
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.120.175.175
        IPv4 Interface Address: 20.120.175.120
        IPv6 Neighbor Address: 2001:0:120:175::175
        Global IPv6 Interface Address: 2001:0:120:175::120
        Adj-sid: 1146 flags: [L V] weight: 0x0
        Adj-sid: 1145 flags: [L V F] weight: 0x0
      Reachability         : 10.0.0.120/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 120 Flags: [N] Algorithm: 0
      Reachability         : 20.120.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 209.209.209.201/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 201 Flags: [N] Algorithm: 0
      Reachability          : 2001:0:30:120::/64 Metric: 0 Type: 1 Up
      Reachability          : 2001:0:53:120::/64 Metric: 0 Type: 1 Up
      Reachability          : 2001:0:120:175::/64 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.120 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  13
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
    0000.0000.0128.00-00       2319  21684   332    268 L2  0000.0000.0128.00-00  <>
      Remaining lifetime received: 1197 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Area addresses: 49.0001
      Topology: 0 (IPv4)
      Topology: 2 (IPv6)
      Interface address: 10.0.0.128
      Interface address: 20.128.175.128
      Interface address: 20.128.217.128
      Interface address: 20.128.157.128
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.128.175.175
        IPv4 Interface Address: 20.128.175.128
        Adj-sid: 48004 flags: [L V] weight: 0x0
      IS Neighbor          : Nokia-SR1-217.00    Metric: 10
        IPv4 Neighbor Address: 20.128.217.217
        IPv4 Interface Address: 20.128.217.128
        Adj-sid: 48005 flags: [L V] weight: 0x0
      IS Neighbor          : Juniper-157-PTX10002-36QDD.00 Metric: 10
        IPv4 Neighbor Address: 20.128.157.157
        IPv4 Interface Address: 20.128.157.128
        Adj-sid: 48006 flags: [L V] weight: 0x0
      Reachability         : 10.0.0.128/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 128 Flags: [N] Algorithm: 0
      Reachability         : 20.128.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.128.217.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.128.157.0/24 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.128 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  10
        SR Capability: Flags: [I]
          SRGB Base: 16000 Range: 4000
 U  Juniper-156-PTX10002-36QDD.00-00      2430  20848   982    297 L2  0000.0000.0156.00-00  <>
      Remaining lifetime received: 1196 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Juniper-156-PTX10002-36QDD
      Area addresses: 49.0001
      Topology: 0 (IPv4)
      Topology: 2 (IPv6)
      Interface address: 10.0.0.156
      Interface address: 209.209.209.201
      Interface address: 2002::156
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 10.156.175.175
        IPv4 Interface Address: 10.156.175.156
        Adj-sid: 36 flags: [L V] weight: 0x0
      Reachability         : 10.0.0.156/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 156 Flags: [N] Algorithm: 0
        SR Prefix-SID: 1286 Flags: [N] Algorithm: 130
        SR Prefix-SID: 1285 Flags: [N] Algorithm: 129
        SR Prefix-SID: 1284 Flags: [N] Algorithm: 128
      Reachability         : 209.209.209.201/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 201 Flags: [] Algorithm: 0
      Reachability         : 10.0.0.30/32 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.156 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  0
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0, 1, 128, 129, 130
      Unsupported TLV: Type: 14 Length: 2
    Juniper-175-ACX7100-48L.00-00      1528  11919  1090   1070 L2  0000.0000.0175.00-00  <>
      Remaining lifetime received: 1198 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Juniper-175-ACX7100-48L
      Area addresses: 49.0001
      Topology: 0 (IPv4)
      Topology: 2 (IPv6)
      Interface address: 10.0.0.175
      Interface address: 127.0.0.1
      Interface address: 2002::175
      IS Neighbor          : Nokia-IXRe2-216.00  Metric: 100
        IPv4 Neighbor Address: 20.175.216.216
        IPv4 Interface Address: 20.175.216.175
        Global IPv6 Interface Address: 2001:0:175:217::175
        Adj-sid: 206 flags: [L V] weight: 0x0
      IS Neighbor          : Arista-PE32-Q2C-32.00 Metric: 50
        IPv4 Neighbor Address: 20.32.175.32
        IPv4 Interface Address: 20.32.175.175
        IPv6 Neighbor Address: 2001:0:32:175::32
        Global IPv6 Interface Address: 2001:0:32:175::175
        Adj-sid: 147 flags: [L V] weight: 0x0
      IS Neighbor          : Juniper-179-ACX7024.00 Metric: 100
        IPv4 Neighbor Address: 20.175.179.179
        IPv4 Interface Address: 20.175.179.175
        IPv6 Neighbor Address: 2001:0:175::179:179
        Global IPv6 Interface Address: 2001:0:175::179:175
        Adj-sid: 213 flags: [L V B] weight: 0x0
      IS Neighbor (MT-IPv6): Arista-PE32-Q2C-32.00 Metric: 10
        IPv4 Interface Address: 20.32.175.175
        IPv6 Neighbor Address: 2001:0:32:175::32
        Global IPv6 Interface Address: 2001:0:32:175::175
        Adj-sid: 148 flags: [L V F] weight: 0x0
      Reachability         : 127.0.0.1/32 Metric: 0 Type: 1 Up
      Reachability         : 10.0.0.175/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 175 Flags: [N] Algorithm: 0
        SR Prefix-SID: 1305 Flags: [N] Algorithm: 130
        SR Prefix-SID: 1304 Flags: [N] Algorithm: 129
        SR Prefix-SID: 1303 Flags: [N] Algorithm: 128
      Reachability         : 20.72.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.175.184.0/24 Metric: 100 Type: 1 Up
      Reachability         : 20.53.175.0/24 Metric: 100 Type: 1 Up
      Reachability         : 20.66.175.0/24 Metric: 100 Type: 1 Up
      Reachability         : 20.175.179.0/24 Metric: 100 Type: 1 Up
      Reachability         : 20.128.175.0/24 Metric: 100 Type: 1 Up
      Reachability         : 20.120.175.0/24 Metric: 100 Type: 1 Up
      Reachability         : 20.175.216.0/24 Metric: 100 Type: 1 Up
      Reachability         : 20.32.175.0/24 Metric: 50 Type: 1 Up
      Reachability         : 20.175.214.0/24 Metric: 75 Type: 1 Up
      Reachability (MT-IPv6): 2002::175/128 Metric: 0 Type: 1 Up
        SR Prefix-SID: 575 Flags: [N] Algorithm: 0
        SR Prefix-SID: 1705 Flags: [N] Algorithm: 130
        SR Prefix-SID: 1704 Flags: [N] Algorithm: 129
        SR Prefix-SID: 1703 Flags: [N] Algorithm: 128
      Reachability (MT-IPv6): 2001:0:175:214::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:66:175::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:72:175::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:32:175::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:175:184::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:128:175::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:175:217::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:120:175::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:175::/64 Metric: 10 Type: 1 Up
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
    Juniper-175-ACX7100-48L.00-01      1268  25982  1090   1071 L2  0000.0000.0175.00-01  <>
      Remaining lifetime received: 1198 s Modified to: 1200 s
      IS Neighbor          : 0000.0000.0128.00   Metric: 100
        IPv4 Neighbor Address: 20.128.175.128
        IPv4 Interface Address: 20.128.175.175
        Global IPv6 Interface Address: 2001:0:128:175::175
        Adj-sid: 215 flags: [L V] weight: 0x0
      IS Neighbor          : Keysight-184.00     Metric: 100
        IPv4 Neighbor Address: 20.175.184.184
        IPv4 Interface Address: 20.175.184.175
        Global IPv6 Interface Address: 2001:0:175:184::175
        Adj-sid: 223 flags: [L V] weight: 0x0
      IS Neighbor          : Nokia-SXR-214.00    Metric: 75
        IPv4 Neighbor Address: 20.175.214.214
        IPv4 Interface Address: 20.175.214.175
        IPv6 Neighbor Address: 2001:0:175:214::214
        Global IPv6 Interface Address: 2001:0:175:214::175
        Adj-sid: 209 flags: [L V] weight: 0x0
      IS Neighbor          : Ciena-8140-66.00    Metric: 100
        IPv4 Neighbor Address: 20.66.175.66
        IPv4 Interface Address: 20.66.175.175
        Global IPv6 Interface Address: 2001:0:66:175::175
        Adj-sid: 224 flags: [L V] weight: 0x0
      IS Neighbor          : 0000.0000.0120.00   Metric: 100
        IPv4 Neighbor Address: 20.120.175.120
        IPv4 Interface Address: 20.120.175.175
        IPv6 Neighbor Address: 2001:0:120:175::120
        Global IPv6 Interface Address: 2001:0:120:175::175
        Adj-sid: 219 flags: [L V] weight: 0x0
      IS Neighbor          : Arrcus-53.00        Metric: 100
        IPv4 Neighbor Address: 20.53.175.53
        IPv4 Interface Address: 20.53.175.175
        IPv6 Neighbor Address: 2001:0:53:175::53
        Global IPv6 Interface Address: 2001:0:53:175::175
        Adj-sid: 216 flags: [L V] weight: 0x0
      IS Neighbor (MT-IPv6): Nokia-SXR-214.00    Metric: 10
        IPv4 Interface Address: 20.175.214.175
        IPv6 Neighbor Address: 2001:0:175:214::214
        Global IPv6 Interface Address: 2001:0:175:214::175
        Adj-sid: 210 flags: [L V F] weight: 0x0
      IS Neighbor (MT-IPv6): Arrcus-53.00        Metric: 10
        IPv4 Interface Address: 20.53.175.175
        IPv6 Neighbor Address: 2001:0:53:175::53
        Global IPv6 Interface Address: 2001:0:53:175::175
        Adj-sid: 217 flags: [L V F] weight: 0x0
      Reachability (MT-IPv6): 2001:0:53:175::/64 Metric: 10 Type: 1 Up
    Juniper-179-ACX7024.00-00      1118  47374   393    327 L2  0000.0000.0179.00-00  <>
      Remaining lifetime received: 1196 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Juniper-179-ACX7024
      Area addresses: 49.0001
      Interface address: 10.0.0.179
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.175.179.175
        IPv4 Interface Address: 20.175.179.179
        IPv6 Neighbor Address: 2001:0:175::179:175
        Global IPv6 Interface Address: 2001:0:175::179:179
        Adj-sid: 99 flags: [L V F] weight: 0x0
        Adj-sid: 98 flags: [L V] weight: 0x0
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
    Keys195.00-00               130  49220  1147    158 L2  0000.0000.0195.00-00  <DefaultAtt>
      Remaining lifetime received: 1198 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6) 0x81(CLNP)
      Hostname: Keys195
      Area addresses:
        49.0001
        49.0001.0000.0000
      Interface address: 20.157.195.195
      IS Neighbor          : Juniper-157-PTX10002-36QDD.00 Metric: 10
      Reachability         : 10.0.0.195/32 Metric: 10 Type: 1 Up
        SR Prefix-SID: 195 Flags: [N] Algorithm: 0
      Reachability         : 10.0.0.195/32 Metric: 10 Type: 1 Up
      Reachability         : 20.157.195.0/24 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.195 Flags: []
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0
    Nokia-SXR-214.00-00       34880  43096   951    402 L2  0000.0000.0214.00-00  <>
      Remaining lifetime received: 1198 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Nokia-SXR-214
      Area addresses: 49.0001
      Topology: 0 (IPv4)
      Topology: 2 (IPv6)
      Interface address: 209.209.209.201
      Interface address: 10.0.0.214
      Interface address: 20.175.214.214
      Interface address: 2000::214
      Interface address: 2001:0:175:214::214
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.175.214.175
        IPv4 Interface Address: 20.175.214.214
        Adj-sid: 30047 flags: [L V] weight: 0x0
      IS Neighbor (MT-IPv6): Juniper-175-ACX7100-48L.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:175:214::175
        Global IPv6 Interface Address: 2001:0:175:214::214
        Adj-sid: 30048 flags: [L V F] weight: 0x0
      Reachability         : 20.175.214.0/24 Metric: 10 Type: 1 Up
      Reachability         : 10.0.0.30/32 Metric: 10 Type: 1 Down
        SR Prefix-SID: 30 Flags: [R N P] Algorithm: 0
      Reachability         : 209.209.209.201/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 201 Flags: [P] Algorithm: 0
      Reachability         : 10.0.0.214/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 214 Flags: [N P] Algorithm: 0
      Reachability (MT-IPv6): 2000::214/128 Metric: 0 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:175:214::/64 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.214 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  15
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0
    Nokia-IXRe2-216.00-00      3678   5095  1117    233 L2  0100.0000.0216.00-00  <>
      Remaining lifetime received: 1198 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Nokia-IXRe2-216
      Area addresses: 49.0001.0000.0000.0216.00
      Topology: 0 (IPv4)
      Topology: 2 (IPv6)
      Interface address: 10.0.0.216
      Interface address: 20.175.216.216
      Interface address: 2002::216
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.175.216.175
        IPv4 Interface Address: 20.175.216.216
        Adj-sid: 1048570 flags: [L V] weight: 0x0
      Reachability         : 20.175.216.0/24 Metric: 10 Type: 1 Up
      Reachability         : 10.0.0.216/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 216 Flags: [N P] Algorithm: 0
      Reachability (MT-IPv6): 2002::216/128 Metric: 0 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.216 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  11
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0
    Nokia-SR1-217.00-00         129  21629   788    225 L2  0100.0000.0217.00-00  <>
      Remaining lifetime received: 1198 s Modified to: 1200 s
      NLPID: 0xCC(IPv4)
      Hostname: Nokia-SR1-217
      Area addresses: 49.0001.0000.0057.00
      Interface address: 10.0.0.217
      Interface address: 20.128.217.217
      Interface address: 20.157.217.217
      IS Neighbor          : Juniper-157-PTX10002-36QDD.00 Metric: 10
        IPv4 Neighbor Address: 20.157.217.157
        IPv4 Interface Address: 20.157.217.217
        Adj-sid: 524269 flags: [L V B] weight: 0x0
      IS Neighbor          : 0000.0000.0128.00   Metric: 10
        IPv4 Neighbor Address: 20.128.217.128
        IPv4 Interface Address: 20.128.217.217
        Adj-sid: 524270 flags: [L V B] weight: 0x0
      Reachability         : 10.0.0.217/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 1217 Flags: [N P] Algorithm: 0
      Reachability         : 20.128.217.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.157.217.0/24 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.217 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  12
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0
 U  221.00-00                   108  24564   648     79 L2  0221.0221.0221.00-00  <>
      Remaining lifetime received: 1198 s Modified to: 1200 s
      NLPID: 0xCC(IPv4)
      Area addresses: 49.0002
      Router Capabilities: Router Id: 10.0.0.221 Flags: []
        SR Local Block:
          SRLB Base: 16 Range: 15344
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  10
        SR Capability: Flags: [I]
          SRGB Base: 20000 Range: 2000
      Unsupported TLV: Type: 14 Length: 2
 U  221.00-01                   105   3577   542     32 L2  0221.0221.0221.00-01  <>
      Remaining lifetime received: 1198 s Modified to: 1200 s
      Hostname: 221
 U  221.00-02                   124  64815   486    205 L2  0221.0221.0221.00-02  <>
      Remaining lifetime received: 1198 s Modified to: 1200 s
      Interface address: 20.175.221.221
      Interface address: 10.0.0.221
      Interface address: 209.209.209.201
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.175.221.175
        IPv4 Interface Address: 20.175.221.221
        Adj-sid: 756646 flags: [L V B] weight: 0x0
        Adj-sid: 756645 flags: [L V] weight: 0x0
      Reachability         : 20.175.221.0/24 Metric: 10 Type: 1 Up
      Reachability         : 10.0.0.221/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 221 Flags: [N] Algorithm: 0
      Reachability         : 209.209.209.201/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 201 Flags: [] Algorithm: 0
    Juniper-157-PTX10002-36QDD.00-00       354  55802   970    358 L2  1000.0000.0157.00-00  <>
      Remaining lifetime received: 1198 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Juniper-157-PTX10002-36QDD
      Area addresses: 49.0001.0000.0000
      Interface address: 10.0.0.157
      Interface address: fe80::3263:eaf0:2f:621b
      IS Neighbor          : 0000.0000.0128.00   Metric: 10
        IPv4 Neighbor Address: 20.128.157.128
        IPv4 Interface Address: 20.128.157.157
        Adj-sid: 26 flags: [L V] weight: 0x0
      IS Neighbor          : Nokia-SR1-217.00    Metric: 10
        IPv4 Neighbor Address: 20.157.217.217
        IPv4 Interface Address: 20.157.217.157
        Adj-sid: 25 flags: [L V] weight: 0x0
      IS Neighbor          : Keys195.00          Metric: 10
        IPv4 Neighbor Address: 20.157.195.195
        IPv4 Interface Address: 20.157.195.157
        Adj-sid: 24 flags: [L V] weight: 0x0
      Reachability         : 20.128.157.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.157.195.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.157.217.0/24 Metric: 10 Type: 1 Up
      Reachability         : 10.0.0.157/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 157 Flags: [N] Algorithm: 0
      Router Capabilities: Router Id: 10.0.0.157 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  0
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0, 1
      Unsupported TLV: Type: 14 Length: 2
    Keysight-184.00-00           12  63668   693    207 L2  6500.0000.0184.00-00  <DefaultAtt>
      Remaining lifetime received: 1197 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6) 0x81(CLNP)
      Hostname: Keysight-184
      Area addresses: 49.0001
      Interface address: 20.175.184.184
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.175.184.175
        IPv4 Interface Address: 20.175.184.184
        Adj-sid: 9001 flags: [L V] weight: 0x0
      Reachability         : 10.0.0.184/32 Metric: 10 Type: 1 Up
        SR Prefix-SID: 184 Flags: [N] Algorithm: 0
      Reachability         : 20.175.184.0/24 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.184 Flags: []
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0

Legend:
H - hostname conflict
U - node unreachable

IS-IS Instance: RIGHT VRF: default
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
    Arista-Spine3-Q2A-30.00-01        98  38964   808    305 L2  0000.0000.0030.00-01  <>
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
      LSP generation remaining wait time: 0 ms
      Time remaining until refresh: 738 s
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
    Nokia-SXR-214.00-00       34879  28493   610    349 L2  0000.0000.0214.00-00  <>
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

IS-IS Instance: LEFT VRF: default
  IS-IS Level 2 Link State Database
    LSPID                   Seq Num  Cksum  Life Length IS  Received LSPID        Flags
    Arista-PE32-Q2C-32.00-00      1147  40403  1064    444 L2  0000.0000.0032.00-00  <>
      LSP generation remaining wait time: 0 ms
      Time remaining until refresh: 764 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Arista-PE32-Q2C-32
      TE IPv4 router ID: 10.0.0.32
      Area addresses: 49.0001
      Topology: 2 (IPv6)
      Topology: 0 (IPv4)
      Interface address: 209.209.209.201
      Interface address: 20.32.175.32
      Interface address: 10.0.0.32
      Interface address: 2001:0:32:175::32
      Interface address: 2002::32
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.32.175.175
        IPv4 Interface Address: 20.32.175.32
        Adj-sid: 362146 flags: [L V] weight: 0x0
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): JUNIPER(1)
            TE default metric: 10
            Min/Max unidirectional link delay: 100000/100000 us
      IS Neighbor (MT-IPv6): Juniper-175-ACX7100-48L.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:32:175::175
        Global IPv6 Interface Address: 2001:0:32:175::32
        Adj-sid: 362147 flags: [L V F] weight: 0x0
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): JUNIPER(1)
            TE default metric: 10
            Min/Max unidirectional link delay: 100000/100000 us
      Reachability         : 10.0.0.30/32 Metric: 10 Type: 1 Down
        SR Prefix-SID: 30 Flags: [R N P] Algorithm: 0
      Reachability         : 209.209.209.201/32 Metric: 10 Type: 1 Up
        SR Prefix-SID: 201 Flags: [P] Algorithm: 0
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
    Arrcus-53.00-00            2274  29619   883    480 L2  0000.0000.0053.00-00  <>
      Remaining lifetime received: 1197 s Modified to: 1200 s
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
      Reachability         : 20.53.66.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.53.72.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.53.120.0/24 Metric: 10 Type: 1 Up
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
    Ciena-8140-66.00-00          22  46217  1107    227 L2  0000.0000.0066.00-00  <>
      Remaining lifetime received: 1197 s Modified to: 1200 s
      NLPID: 0xCC(IPv4)
      Hostname: Ciena-8140-66
      TE IPv4 router ID: 10.0.0.66
      Area addresses: 49.0001
      Topology: 0 (IPv4)
      Interface address: 20.66.175.66
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.66.175.175
        IPv4 Interface Address: 20.66.175.66
        Adj-sid: 16022 flags: [L V] weight: 0x0
        Maximum link BW: 10.00 Gbps
        Maximum reservable link BW: 10.00 Gbps
        Unreserved BW:
            TE class 0: 10.00 Gbps	TE class 1: 10.00 Gbps	TE class 2: 10.00 Gbps
            TE class 3: 10.00 Gbps	TE class 4: 10.00 Gbps	TE class 5: 10.00 Gbps
            TE class 6: 10.00 Gbps	TE class 7: 10.00 Gbps
        Local link ID: 1073731846
        Remote link ID: 1016
        Application Specific Link Attributes:
          Standard applications: [L] RSVP-TE SR-TE LFA Flex-Algo
      Reachability         : 20.66.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 10.0.0.66/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 66 Flags: [N] Algorithm: 0
      Reachability         : 209.209.209.201/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 201 Flags: [] Algorithm: 0
      Router Capabilities: Router Id: 10.0.0.66 Flags: []
        SR Capability: Flags: [I]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0
    0000.0000.0120.00-00        503  41223  1090    372 L2  0000.0000.0120.00-00  <>
      Remaining lifetime received: 1197 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      TE IPv4 router ID: 10.0.0.120
      Area addresses: 49.0000
      Interface address: 10.0.0.120
      Interface address: 20.120.175.120
      Interface address: 209.209.209.201
      Interface address: 2001:0:120:175::120
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.120.175.175
        IPv4 Interface Address: 20.120.175.120
        IPv6 Neighbor Address: 2001:0:120:175::175
        Global IPv6 Interface Address: 2001:0:120:175::120
        Adj-sid: 1146 flags: [L V] weight: 0x0
        Adj-sid: 1145 flags: [L V F] weight: 0x0
        TE default metric: 10
        Maximum link BW: 0.00 bps
        Maximum reservable link BW: 0.00 bps
        Unreserved BW:
            TE class 0: 0.00 bps	TE class 1: 0.00 bps	TE class 2: 0.00 bps
            TE class 3: 0.00 bps	TE class 4: 0.00 bps	TE class 5: 0.00 bps
            TE class 6: 0.00 bps	TE class 7: 0.00 bps
        Local link ID: 1
        Remote link ID: 1007
      Reachability         : 10.0.0.120/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 120 Flags: [N] Algorithm: 0
      Reachability         : 20.120.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 209.209.209.201/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 201 Flags: [N] Algorithm: 0
      Reachability          : 2001:0:30:120::/64 Metric: 0 Type: 1 Up
      Reachability          : 2001:0:53:120::/64 Metric: 0 Type: 1 Up
      Reachability          : 2001:0:120:175::/64 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.120 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  13
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
    0000.0000.0128.00-00       2319  21684   332    268 L2  0000.0000.0128.00-00  <>
      Remaining lifetime received: 1197 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      TE IPv4 router ID: 10.0.0.128
      Area addresses: 49.0001
      Topology: 0 (IPv4)
      Topology: 2 (IPv6)
      Interface address: 10.0.0.128
      Interface address: 20.128.175.128
      Interface address: 20.128.217.128
      Interface address: 20.128.157.128
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.128.175.175
        IPv4 Interface Address: 20.128.175.128
        Adj-sid: 48004 flags: [L V] weight: 0x0
        Local link ID: 9
        Remote link ID: 1011
      IS Neighbor          : Nokia-SR1-217.00    Metric: 10
        IPv4 Neighbor Address: 20.128.217.217
        IPv4 Interface Address: 20.128.217.128
        Adj-sid: 48005 flags: [L V] weight: 0x0
        Local link ID: 8
        Remote link ID: 10
      IS Neighbor          : Juniper-157-PTX10002-36QDD.00 Metric: 10
        IPv4 Neighbor Address: 20.128.157.157
        IPv4 Interface Address: 20.128.157.128
        Adj-sid: 48006 flags: [L V] weight: 0x0
        Local link ID: 13
        Remote link ID: 1048
      Reachability         : 10.0.0.128/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 128 Flags: [N] Algorithm: 0
      Reachability         : 20.128.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.128.217.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.128.157.0/24 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.128 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  10
        SR Capability: Flags: [I]
          SRGB Base: 16000 Range: 4000
 U  Juniper-156-PTX10002-36QDD.00-00      2430  20848   982    297 L2  0000.0000.0156.00-00  <>
      Remaining lifetime received: 1196 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Juniper-156-PTX10002-36QDD
      TE IPv4 router ID: 10.0.0.156
      TE IPv6 router ID: 2002::156
      Area addresses: 49.0001
      Topology: 0 (IPv4)
      Topology: 2 (IPv6)
      Interface address: 10.0.0.156
      Interface address: 209.209.209.201
      Interface address: 2002::156
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 10.156.175.175
        IPv4 Interface Address: 10.156.175.156
        Adj-sid: 36 flags: [L V] weight: 0x0
        Local link ID: 1067
        Remote link ID: 1063
      Reachability         : 10.0.0.156/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 156 Flags: [N] Algorithm: 0
        SR Prefix-SID: 1286 Flags: [N] Algorithm: 130
        SR Prefix-SID: 1285 Flags: [N] Algorithm: 129
        SR Prefix-SID: 1284 Flags: [N] Algorithm: 128
      Reachability         : 209.209.209.201/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 201 Flags: [] Algorithm: 0
      Reachability         : 10.0.0.30/32 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.156 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  0
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0, 1, 128, 129, 130
      Unsupported TLV: Type: 14 Length: 2
    Juniper-175-ACX7100-48L.00-00      1528  11919  1090   1070 L2  0000.0000.0175.00-00  <>
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
      IS Neighbor          : Nokia-IXRe2-216.00  Metric: 100
        IPv4 Neighbor Address: 20.175.216.216
        IPv4 Interface Address: 20.175.216.175
        Global IPv6 Interface Address: 2001:0:175:217::175
        Adj-sid: 206 flags: [L V] weight: 0x0
        TE default metric: 10
        Min/Max unidirectional link delay: 100000/100000 us
        Average unidirectional link delay: 100000 us
        Local link ID: 1003
        Remote link ID: 29
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): JUNIPER(1)
            TE default metric: 10
            Min/Max unidirectional link delay: 100000/100000 us
      IS Neighbor          : Arista-PE32-Q2C-32.00 Metric: 50
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
      IS Neighbor          : Juniper-179-ACX7024.00 Metric: 100
        IPv4 Neighbor Address: 20.175.179.179
        IPv4 Interface Address: 20.175.179.175
        IPv6 Neighbor Address: 2001:0:175::179:179
        Global IPv6 Interface Address: 2001:0:175::179:175
        Adj-sid: 213 flags: [L V B] weight: 0x0
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
      Reachability         : 127.0.0.1/32 Metric: 0 Type: 1 Up
      Reachability         : 10.0.0.175/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 175 Flags: [N] Algorithm: 0
        SR Prefix-SID: 1305 Flags: [N] Algorithm: 130
        SR Prefix-SID: 1304 Flags: [N] Algorithm: 129
        SR Prefix-SID: 1303 Flags: [N] Algorithm: 128
      Reachability         : 20.72.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.175.184.0/24 Metric: 100 Type: 1 Up
      Reachability         : 20.53.175.0/24 Metric: 100 Type: 1 Up
      Reachability         : 20.66.175.0/24 Metric: 100 Type: 1 Up
      Reachability         : 20.175.179.0/24 Metric: 100 Type: 1 Up
      Reachability         : 20.128.175.0/24 Metric: 100 Type: 1 Up
      Reachability         : 20.120.175.0/24 Metric: 100 Type: 1 Up
      Reachability         : 20.175.216.0/24 Metric: 100 Type: 1 Up
      Reachability         : 20.32.175.0/24 Metric: 50 Type: 1 Up
      Reachability         : 20.175.214.0/24 Metric: 75 Type: 1 Up
      Reachability (MT-IPv6): 2002::175/128 Metric: 0 Type: 1 Up
        SR Prefix-SID: 575 Flags: [N] Algorithm: 0
        SR Prefix-SID: 1705 Flags: [N] Algorithm: 130
        SR Prefix-SID: 1704 Flags: [N] Algorithm: 129
        SR Prefix-SID: 1703 Flags: [N] Algorithm: 128
      Reachability (MT-IPv6): 2001:0:175:214::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:66:175::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:72:175::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:32:175::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:175:184::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:128:175::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:175:217::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:120:175::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:175::/64 Metric: 10 Type: 1 Up
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
        Interface Address: 20.175.179.175
        Neighbor Address: 20.175.179.179
        Group ID: 4
      Unsupported TLV: Type: 14 Length: 2
    Juniper-175-ACX7100-48L.00-01      1268  25982  1090   1071 L2  0000.0000.0175.00-01  <>
      Remaining lifetime received: 1198 s Modified to: 1200 s
      IS Neighbor          : 0000.0000.0128.00   Metric: 100
        IPv4 Neighbor Address: 20.128.175.128
        IPv4 Interface Address: 20.128.175.175
        Global IPv6 Interface Address: 2001:0:128:175::175
        Adj-sid: 215 flags: [L V] weight: 0x0
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
      IS Neighbor          : Keysight-184.00     Metric: 100
        IPv4 Neighbor Address: 20.175.184.184
        IPv4 Interface Address: 20.175.184.175
        Global IPv6 Interface Address: 2001:0:175:184::175
        Adj-sid: 223 flags: [L V] weight: 0x0
        TE default metric: 10
        Min/Max unidirectional link delay: 100000/100000 us
        Average unidirectional link delay: 100000 us
        Local link ID: 1012
        Remote link ID: 1
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): JUNIPER(1)
            TE default metric: 10
            Min/Max unidirectional link delay: 100000/100000 us
      IS Neighbor          : Nokia-SXR-214.00    Metric: 75
        IPv4 Neighbor Address: 20.175.214.214
        IPv4 Interface Address: 20.175.214.175
        IPv6 Neighbor Address: 2001:0:175:214::214
        Global IPv6 Interface Address: 2001:0:175:214::175
        Adj-sid: 209 flags: [L V] weight: 0x0
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
      IS Neighbor          : Ciena-8140-66.00    Metric: 100
        IPv4 Neighbor Address: 20.66.175.66
        IPv4 Interface Address: 20.66.175.175
        Global IPv6 Interface Address: 2001:0:66:175::175
        Adj-sid: 224 flags: [L V] weight: 0x0
        TE default metric: 10
        Min/Max unidirectional link delay: 100000/100000 us
        Average unidirectional link delay: 100000 us
        Local link ID: 1016
        Remote link ID: 1073731846
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): JUNIPER(1)
            TE default metric: 10
            Min/Max unidirectional link delay: 100000/100000 us
      IS Neighbor          : 0000.0000.0120.00   Metric: 100
        IPv4 Neighbor Address: 20.120.175.120
        IPv4 Interface Address: 20.120.175.175
        IPv6 Neighbor Address: 2001:0:120:175::120
        Global IPv6 Interface Address: 2001:0:120:175::175
        Adj-sid: 219 flags: [L V] weight: 0x0
        TE default metric: 10
        Min/Max unidirectional link delay: 100000/100000 us
        Average unidirectional link delay: 100000 us
        Local link ID: 1007
        Remote link ID: 1
        Application Specific Link Attributes:
          Standard applications: Flex-Algo
            Administrative group (Color): JUNIPER(1)
            TE default metric: 10
            Min/Max unidirectional link delay: 100000/100000 us
      IS Neighbor          : Arrcus-53.00        Metric: 100
        IPv4 Neighbor Address: 20.53.175.53
        IPv4 Interface Address: 20.53.175.175
        IPv6 Neighbor Address: 2001:0:53:175::53
        Global IPv6 Interface Address: 2001:0:53:175::175
        Adj-sid: 216 flags: [L V] weight: 0x0
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
      IS Neighbor (MT-IPv6): Nokia-SXR-214.00    Metric: 10
        IPv4 Interface Address: 20.175.214.175
        IPv6 Neighbor Address: 2001:0:175:214::214
        Global IPv6 Interface Address: 2001:0:175:214::175
        Adj-sid: 210 flags: [L V F] weight: 0x0
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
      IS Neighbor (MT-IPv6): Arrcus-53.00        Metric: 10
        IPv4 Interface Address: 20.53.175.175
        IPv6 Neighbor Address: 2001:0:53:175::53
        Global IPv6 Interface Address: 2001:0:53:175::175
        Adj-sid: 217 flags: [L V F] weight: 0x0
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
      Reachability (MT-IPv6): 2001:0:53:175::/64 Metric: 10 Type: 1 Up
    Juniper-179-ACX7024.00-00      1118  47374   393    327 L2  0000.0000.0179.00-00  <>
      Remaining lifetime received: 1196 s Modified to: 1200 s
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
        Adj-sid: 99 flags: [L V F] weight: 0x0
        Adj-sid: 98 flags: [L V] weight: 0x0
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
    Keys195.00-00               130  49220  1147    158 L2  0000.0000.0195.00-00  <DefaultAtt>
      Remaining lifetime received: 1198 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6) 0x81(CLNP)
      Hostname: Keys195
      Area addresses:
        49.0001
        49.0001.0000.0000
      Interface address: 20.157.195.195
      IS Neighbor          : Juniper-157-PTX10002-36QDD.00 Metric: 10
      Reachability         : 10.0.0.195/32 Metric: 10 Type: 1 Up
        SR Prefix-SID: 195 Flags: [N] Algorithm: 0
      Reachability         : 10.0.0.195/32 Metric: 10 Type: 1 Up
      Reachability         : 20.157.195.0/24 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.195 Flags: []
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0
    Nokia-SXR-214.00-00       34880  43096   951    402 L2  0000.0000.0214.00-00  <>
      Remaining lifetime received: 1198 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Nokia-SXR-214
      TE IPv4 router ID: 10.0.0.214
      TE IPv6 router ID: 2000::214
      Area addresses: 49.0001
      Topology: 0 (IPv4)
      Topology: 2 (IPv6)
      Interface address: 209.209.209.201
      Interface address: 10.0.0.214
      Interface address: 20.175.214.214
      Interface address: 2000::214
      Interface address: 2001:0:175:214::214
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.175.214.175
        IPv4 Interface Address: 20.175.214.214
        Adj-sid: 30047 flags: [L V] weight: 0x0
        TE default metric: 10
        Maximum link BW: 80.00 Mbps
        Application Specific Link Attributes:
          Standard applications: [L] SR-TE
      IS Neighbor (MT-IPv6): Juniper-175-ACX7100-48L.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:175:214::175
        Global IPv6 Interface Address: 2001:0:175:214::214
        Adj-sid: 30048 flags: [L V F] weight: 0x0
        TE default metric: 10
        Maximum link BW: 80.00 Mbps
        Application Specific Link Attributes:
          Standard applications: [L] SR-TE
      Reachability         : 20.175.214.0/24 Metric: 10 Type: 1 Up
      Reachability         : 10.0.0.30/32 Metric: 10 Type: 1 Down
        SR Prefix-SID: 30 Flags: [R N P] Algorithm: 0
      Reachability         : 209.209.209.201/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 201 Flags: [P] Algorithm: 0
      Reachability         : 10.0.0.214/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 214 Flags: [N P] Algorithm: 0
      Reachability (MT-IPv6): 2000::214/128 Metric: 0 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:175:214::/64 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.214 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  15
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0
    Nokia-IXRe2-216.00-00      3678   5095  1117    233 L2  0100.0000.0216.00-00  <>
      Remaining lifetime received: 1198 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Nokia-IXRe2-216
      TE IPv4 router ID: 10.0.0.216
      TE IPv6 router ID: 2002::216
      Area addresses: 49.0001.0000.0000.0216.00
      Topology: 0 (IPv4)
      Topology: 2 (IPv6)
      Interface address: 10.0.0.216
      Interface address: 20.175.216.216
      Interface address: 2002::216
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.175.216.175
        IPv4 Interface Address: 20.175.216.216
        Adj-sid: 1048570 flags: [L V] weight: 0x0
      Reachability         : 20.175.216.0/24 Metric: 10 Type: 1 Up
      Reachability         : 10.0.0.216/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 216 Flags: [N P] Algorithm: 0
      Reachability (MT-IPv6): 2002::216/128 Metric: 0 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.216 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  11
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0
    Nokia-SR1-217.00-00         129  21629   788    225 L2  0100.0000.0217.00-00  <>
      Remaining lifetime received: 1198 s Modified to: 1200 s
      NLPID: 0xCC(IPv4)
      Hostname: Nokia-SR1-217
      TE IPv4 router ID: 10.0.0.217
      Area addresses: 49.0001.0000.0057.00
      Interface address: 10.0.0.217
      Interface address: 20.128.217.217
      Interface address: 20.157.217.217
      IS Neighbor          : Juniper-157-PTX10002-36QDD.00 Metric: 10
        IPv4 Neighbor Address: 20.157.217.157
        IPv4 Interface Address: 20.157.217.217
        Adj-sid: 524269 flags: [L V B] weight: 0x0
      IS Neighbor          : 0000.0000.0128.00   Metric: 10
        IPv4 Neighbor Address: 20.128.217.128
        IPv4 Interface Address: 20.128.217.217
        Adj-sid: 524270 flags: [L V B] weight: 0x0
      Reachability         : 10.0.0.217/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 1217 Flags: [N P] Algorithm: 0
      Reachability         : 20.128.217.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.157.217.0/24 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.217 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  12
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0
 U  221.00-00                   108  24564   648     79 L2  0221.0221.0221.00-00  <>
      Remaining lifetime received: 1198 s Modified to: 1200 s
      NLPID: 0xCC(IPv4)
      TE IPv4 router ID: 10.0.0.221
      Area addresses: 49.0002
      Router Capabilities: Router Id: 10.0.0.221 Flags: []
        SR Local Block:
          SRLB Base: 16 Range: 15344
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  10
        SR Capability: Flags: [I]
          SRGB Base: 20000 Range: 2000
      Unsupported TLV: Type: 14 Length: 2
 U  221.00-01                   105   3577   542     32 L2  0221.0221.0221.00-01  <>
      Remaining lifetime received: 1198 s Modified to: 1200 s
      Hostname: 221
 U  221.00-02                   124  64815   486    205 L2  0221.0221.0221.00-02  <>
      Remaining lifetime received: 1198 s Modified to: 1200 s
      Interface address: 20.175.221.221
      Interface address: 10.0.0.221
      Interface address: 209.209.209.201
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.175.221.175
        IPv4 Interface Address: 20.175.221.221
        Adj-sid: 756646 flags: [L V B] weight: 0x0
        Adj-sid: 756645 flags: [L V] weight: 0x0
        Administrative group (Color): JUNIPER(1)
        TE default metric: 10
        Maximum link BW: 10.00 Gbps
        Maximum reservable link BW: 10.00 Gbps
        Unreserved BW:
            TE class 0: 10.00 Gbps	TE class 1: 10.00 Gbps	TE class 2: 10.00 Gbps
            TE class 3: 10.00 Gbps	TE class 4: 10.00 Gbps	TE class 5: 10.00 Gbps
            TE class 6: 10.00 Gbps	TE class 7: 10.00 Gbps
        Min/Max unidirectional link delay: 10/10 us
      Reachability         : 20.175.221.0/24 Metric: 10 Type: 1 Up
      Reachability         : 10.0.0.221/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 221 Flags: [N] Algorithm: 0
      Reachability         : 209.209.209.201/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 201 Flags: [] Algorithm: 0
    Juniper-157-PTX10002-36QDD.00-00       354  55802   970    358 L2  1000.0000.0157.00-00  <>
      Remaining lifetime received: 1198 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Juniper-157-PTX10002-36QDD
      TE IPv4 router ID: 10.0.0.157
      TE IPv6 router ID: fe80::3263:eaf0:2f:621b
      Area addresses: 49.0001.0000.0000
      Interface address: 10.0.0.157
      Interface address: fe80::3263:eaf0:2f:621b
      IS Neighbor          : 0000.0000.0128.00   Metric: 10
        IPv4 Neighbor Address: 20.128.157.128
        IPv4 Interface Address: 20.128.157.157
        Adj-sid: 26 flags: [L V] weight: 0x0
        Local link ID: 1048
        Remote link ID: 13
      IS Neighbor          : Nokia-SR1-217.00    Metric: 10
        IPv4 Neighbor Address: 20.157.217.217
        IPv4 Interface Address: 20.157.217.157
        Adj-sid: 25 flags: [L V] weight: 0x0
        Local link ID: 1004
        Remote link ID: 11
      IS Neighbor          : Keys195.00          Metric: 10
        IPv4 Neighbor Address: 20.157.195.195
        IPv4 Interface Address: 20.157.195.157
        Adj-sid: 24 flags: [L V] weight: 0x0
        Local link ID: 1040
        Remote link ID: 1
      Reachability         : 20.128.157.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.157.195.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.157.217.0/24 Metric: 10 Type: 1 Up
      Reachability         : 10.0.0.157/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 157 Flags: [N] Algorithm: 0
      Router Capabilities: Router Id: 10.0.0.157 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  0
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0, 1
      Unsupported TLV: Type: 14 Length: 2
    Keysight-184.00-00           12  63668   693    207 L2  6500.0000.0184.00-00  <DefaultAtt>
      Remaining lifetime received: 1197 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6) 0x81(CLNP)
      Hostname: Keysight-184
      TE IPv4 router ID: 10.0.0.184
      Area addresses: 49.0001
      Interface address: 20.175.184.184
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.175.184.175
        IPv4 Interface Address: 20.175.184.184
        Adj-sid: 9001 flags: [L V] weight: 0x0
        TE default metric: 0
        Maximum link BW: 1.00 Gbps
        Maximum reservable link BW: 1.00 Gbps
        Unreserved BW:
            TE class 0: 1.00 Gbps	TE class 1: 1.00 Gbps	TE class 2: 1.00 Gbps
            TE class 3: 1.00 Gbps	TE class 4: 1.00 Gbps	TE class 5: 1.00 Gbps
            TE class 6: 1.00 Gbps	TE class 7: 1.00 Gbps
      Reachability         : 10.0.0.184/32 Metric: 10 Type: 1 Up
        SR Prefix-SID: 184 Flags: [N] Algorithm: 0
      Reachability         : 20.175.184.0/24 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.184 Flags: []
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0

Legend:
H - hostname conflict
U - node unreachable

IS-IS Instance: RIGHT VRF: default
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
    Arista-Spine3-Q2A-30.00-01        98  38964   807    305 L2  0000.0000.0030.00-01  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
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
      LSP generation remaining wait time: 0 ms
      Time remaining until refresh: 738 s
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
    Nokia-SXR-214.00-00       34879  28493   610    349 L2  0000.0000.0214.00-00  <>
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
 U  221.00-00                   107  11306   431     79 L2  0221.0221.0221.00-00  <>
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
   Destination                   Algorithm         Next Hop         Interface
----------------------------- ----------------- ------------------- ---------
   Arista-PE32-Q2C-32            MIN-LATENCY                                 
                                                                             
   Arista-PE32-Q2C-32            MIN-TE                                      
                                                                             
   Arista-PE32-Q2C-32            ADMIN                                       
                                                                             
   Arrcus-53                     MIN-LATENCY       20.32.175.175    Ethernet5
                                                                             
   Arrcus-53                     MIN-TE            20.32.175.175    Ethernet5
                                                                             
   Arrcus-53                     ADMIN                                       
                                                                             
   Juniper-175-ACX7100-48L       MIN-LATENCY       20.32.175.175    Ethernet5
                                                                             
   Juniper-175-ACX7100-48L       MIN-TE            20.32.175.175    Ethernet5
                                                                             
   Juniper-175-ACX7100-48L       ADMIN                                       
                                                                             
   Juniper-179-ACX7024           MIN-LATENCY       20.32.175.175    Ethernet5
                                                                             
   Juniper-179-ACX7024           MIN-TE            20.32.175.175    Ethernet5
                                                                             
   Juniper-179-ACX7024           ADMIN                                       
                                                                             

Flex algo paths for IPv6 address family
Topology ID: Level-2
 Destination               Algorithm      Next Hop                    Interface
------------------------- -------------- ---------------------------- ---------
 Arrcus-53                 MIN-LATENCY    fe80::3e08:cdff:fe8d:badc   Ethernet5
                                                                               
 Arrcus-53                 MIN-TE         fe80::3e08:cdff:fe8d:badc   Ethernet5
                                                                               
 Arrcus-53                 ADMIN                                               
                                                                               
 Juniper-175-ACX7100-48L   MIN-LATENCY    fe80::3e08:cdff:fe8d:badc   Ethernet5
                                                                               
 Juniper-175-ACX7100-48L   MIN-TE         fe80::3e08:cdff:fe8d:badc   Ethernet5
                                                                               
 Juniper-175-ACX7100-48L   ADMIN                                               
                                                                               

```

## show isis flex-algo path detail

```text
Flex algo paths for IPv4 address family
Topology ID: Level-2
Destination: Arista-PE32-Q2C-32
Path ID: 66176
Path constraints: algo MIN-LATENCY
                  metric type MIN-DELAY
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 1
Last updated: 17:42:47 ago
Next Hop Interface
-------- ---------

Destination: Arista-PE32-Q2C-32
Path ID: 66177
Path constraints: algo MIN-TE
                  metric type TE
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 1
Last updated: 17:42:47 ago
Next Hop Interface
-------- ---------

Destination: Arista-PE32-Q2C-32
Path ID: 66178
Path constraints: algo ADMIN
                  metric type IGP
                  administrative-group exclude JUNIPER(1)
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 1
Last updated: 17:42:47 ago
Next Hop Interface
-------- ---------

Destination: Arrcus-53
Path ID: 66176
Path constraints: algo MIN-LATENCY
                  metric type MIN-DELAY
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 1
Last updated: 16:00:27 ago
Metric: 200000
Next Hop      Interface
------------- ---------
20.32.175.175 Ethernet5

Destination: Arrcus-53
Path ID: 66177
Path constraints: algo MIN-TE
                  metric type TE
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 1
Last updated: 16:00:27 ago
Metric: 20
Next Hop      Interface
------------- ---------
20.32.175.175 Ethernet5

Destination: Arrcus-53
Path ID: 66178
Path constraints: algo ADMIN
                  metric type IGP
                  administrative-group exclude JUNIPER(1)
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 1
Last updated: 16:00:27 ago
Next Hop Interface
-------- ---------

Destination: Juniper-175-ACX7100-48L
Path ID: 66176
Path constraints: algo MIN-LATENCY
                  metric type MIN-DELAY
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 1
Last updated: 17:42:47 ago
Metric: 100000
Next Hop      Interface
------------- ---------
20.32.175.175 Ethernet5

Destination: Juniper-175-ACX7100-48L
Path ID: 66177
Path constraints: algo MIN-TE
                  metric type TE
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 1
Last updated: 17:42:47 ago
Metric: 10
Next Hop      Interface
------------- ---------
20.32.175.175 Ethernet5

Destination: Juniper-175-ACX7100-48L
Path ID: 66178
Path constraints: algo ADMIN
                  metric type IGP
                  administrative-group exclude JUNIPER(1)
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 1
Last updated: 17:42:47 ago
Next Hop Interface
-------- ---------

Destination: Juniper-179-ACX7024
Path ID: 66176
Path constraints: algo MIN-LATENCY
                  metric type MIN-DELAY
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 1
Last updated: 17:42:35 ago
Metric: 200000
Next Hop      Interface
------------- ---------
20.32.175.175 Ethernet5

Destination: Juniper-179-ACX7024
Path ID: 66177
Path constraints: algo MIN-TE
                  metric type TE
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 1
Last updated: 17:42:35 ago
Metric: 20
Next Hop      Interface
------------- ---------
20.32.175.175 Ethernet5

Destination: Juniper-179-ACX7024
Path ID: 66178
Path constraints: algo ADMIN
                  metric type IGP
                  administrative-group exclude JUNIPER(1)
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 1
Last updated: 17:42:35 ago
Next Hop Interface
-------- ---------

Flex algo paths for IPv6 address family
Topology ID: Level-2
Destination: Arrcus-53
Path ID: 66176
Path constraints: algo MIN-LATENCY
                  metric type MIN-DELAY
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 1
Last updated: 16:00:27 ago
Metric: 200000
Next Hop                  Interface
------------------------- ---------
fe80::3e08:cdff:fe8d:badc Ethernet5

Destination: Arrcus-53
Path ID: 66177
Path constraints: algo MIN-TE
                  metric type TE
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 1
Last updated: 16:00:27 ago
Metric: 20
Next Hop                  Interface
------------------------- ---------
fe80::3e08:cdff:fe8d:badc Ethernet5

Destination: Arrcus-53
Path ID: 66178
Path constraints: algo ADMIN
                  metric type IGP
                  administrative-group exclude JUNIPER(1)
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 1
Last updated: 16:00:27 ago
Next Hop Interface
-------- ---------

Destination: Juniper-175-ACX7100-48L
Path ID: 66176
Path constraints: algo MIN-LATENCY
                  metric type MIN-DELAY
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 1
Last updated: 17:42:47 ago
Metric: 100000
Next Hop                  Interface
------------------------- ---------
fe80::3e08:cdff:fe8d:badc Ethernet5

Destination: Juniper-175-ACX7100-48L
Path ID: 66177
Path constraints: algo MIN-TE
                  metric type TE
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 1
Last updated: 17:42:47 ago
Metric: 10
Next Hop                  Interface
------------------------- ---------
fe80::3e08:cdff:fe8d:badc Ethernet5

Destination: Juniper-175-ACX7100-48L
Path ID: 66178
Path constraints: algo ADMIN
                  metric type IGP
                  administrative-group exclude JUNIPER(1)
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 1
Last updated: 17:42:47 ago
Next Hop Interface
-------- ---------

```

## show isis segment-routing tunnel

```text
 Index    Endpoint          Next Hop/Tunnel Index         Interface   Labels   
-------- ---------------- ----------------------------- ------------- ---------
 1        10.0.0.30/32      20.30.32.30                   Ethernet1   [ 3 ]    
 2        2002::30/128      fe80::c6ca:2bff:fe45:a215     Ethernet1   [ 3 ]    
 3        10.0.0.84/32      20.30.32.30                   Ethernet1   [ 20084 ]
 4        10.0.0.72/32      20.30.32.30                   Ethernet1   [ 20072 ]
 5        10.0.0.175/32     20.32.175.175                 Ethernet5   [ 3 ]    
 7        10.0.0.214/32     20.32.175.175                 Ethernet5   [ 20214 ]
 9        2002::175/128     fe80::3e08:cdff:fe8d:badc     Ethernet5   [ 3 ]    
 10       10.0.0.128/32     20.32.175.175                 Ethernet5   [ 20128 ]
 11       10.0.0.53/32      20.32.175.175                 Ethernet5   [ 20053 ]
 12       10.0.0.179/32     20.32.175.175                 Ethernet5   [ 20179 ]
 13       2002::53/128      fe80::3e08:cdff:fe8d:badc     Ethernet5   [ 20453 ]
 14       10.0.0.184/32     20.32.175.175                 Ethernet5   [ 20184 ]
 15       10.0.0.216/32     20.32.175.175                 Ethernet5   [ 20216 ]
 16       10.0.0.31/32      20.30.32.30                   Ethernet1   [ 20031 ]
 17       10.0.0.120/32     20.30.32.30                   Ethernet1   [ 20120 ]
 18       10.0.0.157/32     20.32.175.175                 Ethernet5   [ 20157 ]
 19       10.0.0.195/32     20.32.175.175                 Ethernet5   [ 20195 ]
 20       10.0.0.217/32     20.32.175.175                 Ethernet5   [ 21217 ]
 21       10.0.0.122/32     20.30.32.30                   Ethernet1   [ 20122 ]
 22       10.0.0.66/32      20.32.175.175                 Ethernet5   [ 20066 ]

```

## show isis segment-routing prefix-segments

```text

System ID: Arista-PE32-Q2C-32			Instance: 'LEFT'
SR supported Data-plane: MPLS			SR Router ID: 10.0.0.32

Node: 31     Proxy-Node: 0      Prefix: 1       Total Segments: 32

Flag Descriptions: R: Re-advertised, N: Node Segment, P: no-PHP
                   E: Explicit-NULL, V: Value, L: Local
Segment status codes: * - Self originated Prefix, L1 - level 1, L2 - level 2, ! - SR-unreachable,
                      # - Some IS-IS next-hops are SR-unreachable
   Prefix                      SID   Label Type       Flags                        System ID       Level Protection  Algorithm   
   ------------------------- ----- ------- ---------- ---------------------------- --------------- ----- ----------- -------------
*  10.0.0.32/32                161   20161 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-PE32-Q2C-32 L2    unprotected MIN-LATENCY 
*  10.0.0.32/32                162   20162 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-PE32-Q2C-32 L2    unprotected MIN-TE      
*  10.0.0.32/32                163   20163 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-PE32-Q2C-32 L2    unprotected ADMIN       
   10.0.0.53/32                 53   20053 Node       R:0 N:1 P:1 E:1 V:0 L:0      Arrcus-53       L2    node with SRLG strict SPF         
   10.0.0.53/32               1181   21181 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arrcus-53       L2    node with SRLG strict MIN-LATENCY 
   10.0.0.53/32               1182   21182 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arrcus-53       L2    node with SRLG strict MIN-TE      
   10.0.0.53/32               1183   21183 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arrcus-53       L2    unprotected ADMIN       
   10.0.0.66/32                 66   20066 Node       R:0 N:1 P:0 E:0 V:0 L:0      Ciena-8140-66   L2    node with SRLG strict SPF         
   10.0.0.128/32               128   16128 Node       R:0 N:1 P:0 E:0 V:0 L:0      0000.0000.0128  L2    node with SRLG strict SPF         
   10.0.0.157/32               157   20157 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-157-PTX10002-36QDD L2    node with SRLG strict SPF         
   10.0.0.175/32               175   20175 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-175-ACX7100-48L L2    node with SRLG strict SPF         
   10.0.0.175/32              1303   21303 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-175-ACX7100-48L L2    node with SRLG strict MIN-LATENCY 
   10.0.0.175/32              1304   21304 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-175-ACX7100-48L L2    node with SRLG strict MIN-TE      
   10.0.0.175/32              1305   21305 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-175-ACX7100-48L L2    unprotected ADMIN       
   10.0.0.179/32               179   20179 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-179-ACX7024 L2    node with SRLG strict SPF         
   10.0.0.179/32              1307   21307 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-179-ACX7024 L2    node with SRLG strict MIN-LATENCY 
   10.0.0.179/32              1308   21308 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-179-ACX7024 L2    node with SRLG strict MIN-TE      
   10.0.0.179/32              1309   21309 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-179-ACX7024 L2    unprotected ADMIN       
   10.0.0.184/32               184   20184 Node       R:0 N:1 P:0 E:0 V:0 L:0      Keysight-184    L2    node with SRLG strict SPF         
   10.0.0.195/32               195   20195 Node       R:0 N:1 P:0 E:0 V:0 L:0      Keys195         L2    node with SRLG strict SPF         
   10.0.0.214/32               214   20214 Node       R:0 N:1 P:1 E:0 V:0 L:0      Nokia-SXR-214   L2    node with SRLG strict SPF         
   10.0.0.216/32               216   20216 Node       R:0 N:1 P:1 E:0 V:0 L:0      Nokia-IXRe2-216 L2    node with SRLG strict SPF         
   10.0.0.217/32              1217   21217 Node       R:0 N:1 P:1 E:0 V:0 L:0      Nokia-SR1-217   L2    node with SRLG strict SPF         
   209.209.209.201/32          201   20201 Prefix     R:0 N:0 P:1 E:0 V:0 L:0      Nokia-SXR-214   L2    unprotected SPF         
*  209.209.209.201/32          201   20201 Prefix     R:0 N:0 P:1 E:0 V:0 L:0      Arista-PE32-Q2C-32 L2    unprotected SPF         
   209.209.209.201/32          201   20201 Prefix     R:0 N:0 P:1 E:0 V:0 L:0      Ciena-8140-66   L2    unprotected SPF         
   209.209.209.201/32          201   20201 Prefix     R:0 N:0 P:1 E:0 V:0 L:0      0000.0000.0120  L2    unprotected SPF         
   2002::53/128                453   20453 Node       R:0 N:1 P:1 E:1 V:0 L:0      Arrcus-53       L2    node        SPF         
   2002::53/128               1581   21581 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arrcus-53       L2    node        MIN-LATENCY 
   2002::53/128               1582   21582 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arrcus-53       L2    node        MIN-TE      
   2002::53/128               1583   21583 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arrcus-53       L2    unprotected ADMIN       
   2002::175/128               575   20575 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-175-ACX7100-48L L2    node        SPF         
   2002::175/128              1703   21703 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-175-ACX7100-48L L2    node        MIN-LATENCY 
   2002::175/128              1704   21704 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-175-ACX7100-48L L2    node        MIN-TE      
   2002::175/128              1705   21705 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-175-ACX7100-48L L2    unprotected ADMIN       

System ID: Arista-PE32-Q2C-32			Instance: 'RIGHT'
SR supported Data-plane: MPLS			SR Router ID: 10.0.0.32

Node: 13     Proxy-Node: 0      Prefix: 2       Total Segments: 15

Flag Descriptions: R: Re-advertised, N: Node Segment, P: no-PHP
                   E: Explicit-NULL, V: Value, L: Local
Segment status codes: * - Self originated Prefix, L1 - level 1, L2 - level 2, ! - SR-unreachable,
                      # - Some IS-IS next-hops are SR-unreachable
   Prefix                      SID   Label Type       Flags                        System ID       Level Protection  Algorithm   
   ------------------------- ----- ------- ---------- ---------------------------- --------------- ----- ----------- -------------
   10.0.0.30/32                 30   20030 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-Spine3-Q2A-30 L2    node        SPF         
   10.0.0.30/32                158   20158 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-Spine3-Q2A-30 L2    unprotected MIN-LATENCY 
   10.0.0.30/32                159   20159 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-Spine3-Q2A-30 L2    unprotected MIN-TE      
   10.0.0.30/32                160   20160 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-Spine3-Q2A-30 L2    unprotected ADMIN       
   10.0.0.31/32                 31   20031 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-PE31-Q2C-31 L2    node        SPF         
*  10.0.0.32/32                 32   20032 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-PE32-Q2C-32 L2    unprotected SPF         
   10.0.0.72/32                 72   20072 Node       R:0 N:1 P:0 E:0 V:0 L:0      Ciena-5134-72   L2    node        SPF         
   10.0.0.84/32                 84   20084 Node       R:0 N:1 P:1 E:0 V:0 L:0      Ericsson_84_R6678 L2    node        SPF         
   10.0.0.120/32               120   20120 Prefix     R:1 N:0 P:1 E:0 V:0 L:0      0000.0000.0120  L2    node        SPF         
   10.0.0.122/32               122   20122 Node       R:0 N:1 P:0 E:0 V:0 L:0      0000.0000.0122  L2    node        SPF         
   209.209.209.202/32          202   20202 Prefix     R:0 N:0 P:1 E:0 V:0 L:0      Nokia-SXR-214   L2    unprotected SPF         
*  209.209.209.202/32          202   20202 Prefix     R:0 N:0 P:1 E:0 V:0 L:0      Arista-PE32-Q2C-32 L2    unprotected SPF         
   209.209.209.202/32          202   20202 Prefix     R:0 N:0 P:1 E:0 V:0 L:0      0000.0000.0120  L2    unprotected SPF         
   2002::30/128                430   20430 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-Spine3-Q2A-30 L2    node        SPF         
   2002::30/128                558   20558 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-Spine3-Q2A-30 L2    unprotected MIN-LATENCY 
   2002::30/128                559   20559 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-Spine3-Q2A-30 L2    unprotected MIN-TE      
   2002::30/128                560   20560 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-Spine3-Q2A-30 L2    unprotected ADMIN       
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
 I L2     10.0.0.31/32 [115/85]
           via 20.30.32.30, Ethernet1
 C        10.0.0.32/32
           directly connected, Loopback0
 I L2     10.0.0.53/32 [115/110]
           via 20.32.175.175, Ethernet5
 I L2     10.0.0.66/32 [115/110]
           via 20.30.32.30, Ethernet1
 I L2     10.0.0.72/32 [115/120]
           via 20.30.32.30, Ethernet1
 I L2     10.0.0.84/32 [115/120]
           via 20.30.32.30, Ethernet1
 I L2     10.0.0.120/32 [115/110]
           via 20.30.32.30, Ethernet1
 I L2     10.0.0.122/32 [115/110]
           via 20.30.32.30, Ethernet1
 I L2     10.0.0.128/32 [115/110]
           via 20.32.175.175, Ethernet5
 I L2     10.0.0.157/32 [115/120]
           via 20.32.175.175, Ethernet5
 I L2     10.0.0.175/32 [115/10]
           via 20.32.175.175, Ethernet5
 I L2     10.0.0.179/32 [115/110]
           via 20.32.175.175, Ethernet5
 I L2     10.0.0.184/32 [115/120]
           via 20.32.175.175, Ethernet5
 I L2     10.0.0.195/32 [115/140]
           via 20.32.175.175, Ethernet5
 I L2     10.0.0.214/32 [115/85]
           via 20.32.175.175, Ethernet5
 I L2     10.0.0.216/32 [115/110]
           via 20.32.175.175, Ethernet5
 I L2     10.0.0.217/32 [115/120]
           via 20.32.175.175, Ethernet5
 I L2     20.30.31.0/24 [115/85]
           via 20.30.32.30, Ethernet1
 C        20.30.32.0/24
           directly connected, Ethernet1
 I L2     20.30.66.0/24 [115/110]
           via 20.30.32.30, Ethernet1
 I L2     20.30.72.0/24 [115/110]
           via 20.30.32.30, Ethernet1
 I L2     20.30.84.0/24 [115/110]
           via 20.30.32.30, Ethernet1
 I L2     20.30.120.0/24 [115/110]
           via 20.30.32.30, Ethernet1
 I L2     20.30.122.0/24 [115/110]
           via 20.30.32.30, Ethernet1
 I L2     20.30.214.0/24 [115/110]
           via 20.30.32.30, Ethernet1
 C        20.32.175.0/24
           directly connected, Ethernet5
 I L2     20.53.66.0/24 [115/120]
           via 20.32.175.175, Ethernet5
 I L2     20.53.72.0/24 [115/120]
           via 20.32.175.175, Ethernet5
 I L2     20.53.120.0/24 [115/120]
           via 20.32.175.175, Ethernet5
 I L2     20.53.175.0/24 [115/110]
           via 20.32.175.175, Ethernet5
 I L2     20.66.175.0/24 [115/110]
           via 20.32.175.175, Ethernet5
 I L2     20.72.175.0/24 [115/20]
           via 20.32.175.175, Ethernet5
 I L2     20.120.175.0/24 [115/110]
           via 20.32.175.175, Ethernet5
 I L2     20.128.157.0/24 [115/120]
           via 20.32.175.175, Ethernet5
 I L2     20.128.175.0/24 [115/110]
           via 20.32.175.175, Ethernet5
 I L2     20.128.217.0/24 [115/120]
           via 20.32.175.175, Ethernet5
 I L2     20.157.195.0/24 [115/130]
           via 20.32.175.175, Ethernet5
 I L2     20.157.217.0/24 [115/130]
           via 20.32.175.175, Ethernet5
 I L2     20.175.179.0/24 [115/110]
           via 20.32.175.175, Ethernet5
 I L2     20.175.184.0/24 [115/110]
           via 20.32.175.175, Ethernet5
 I L2     20.175.214.0/24 [115/85]
           via 20.32.175.175, Ethernet5
 I L2     20.175.216.0/24 [115/110]
           via 20.32.175.175, Ethernet5
 I L2     30.122.190.0/24 [115/110]
           via 20.30.32.30, Ethernet1
 I L2     101.64.122.0/24 [115/110]
           via 20.30.32.30, Ethernet1
 I L2     101.74.122.0/24 [115/110]
           via 20.30.32.30, Ethernet1
 I L2     101.88.122.0/24 [115/110]
           via 20.30.32.30, Ethernet1
 I L2     101.119.122.0/24 [115/110]
           via 20.30.32.30, Ethernet1
 I L2     101.122.125.0/24 [115/110]
           via 20.30.32.30, Ethernet1
 I L2     101.122.130.0/24 [115/110]
           via 20.30.32.30, Ethernet1
 I L2     101.122.158.0/24 [115/110]
           via 20.30.32.30, Ethernet1
 I L2     101.122.162.0/24 [115/110]
           via 20.30.32.30, Ethernet1
 I L2     101.122.169.0/24 [115/110]
           via 20.30.32.30, Ethernet1
 I L2     101.122.216.0/24 [115/110]
           via 20.30.32.30, Ethernet1
 I L2     101.122.218.0/24 [115/110]
           via 20.30.32.30, Ethernet1
 C        209.209.209.201/32
           directly connected, Loopback201
 C        209.209.209.202/32
           directly connected, Loopback202


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
Displaying 23 of 28 IPv6 routing table entries
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
 I L2     2001:0:30:31::/64 [115/20]
           via fe80::c6ca:2bff:fe45:a215, Ethernet1
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
 I L2     2001:0:30:214::/64 [115/20]
           via fe80::c6ca:2bff:fe45:a215, Ethernet1
 C        2001:0:32:175::/64 [0/0]
           via Ethernet5, directly connected
 I L2     2001:0:53:175::/64 [115/20]
           via fe80::3e08:cdff:fe8d:badc, Ethernet5
 I L2     2001:0:66:175::/64 [115/20]
           via fe80::3e08:cdff:fe8d:badc, Ethernet5
 I L2     2001:0:72:175::/64 [115/20]
           via fe80::3e08:cdff:fe8d:badc, Ethernet5
 I L2     2001:0:120:175::/64 [115/20]
           via fe80::3e08:cdff:fe8d:badc, Ethernet5
 I L2     2001:0:128:175::/64 [115/20]
           via fe80::3e08:cdff:fe8d:badc, Ethernet5
 I L2     2001:0:175::/64 [115/20]
           via fe80::3e08:cdff:fe8d:badc, Ethernet5
 I L2     2001:0:175:184::/64 [115/20]
           via fe80::3e08:cdff:fe8d:badc, Ethernet5
 I L2     2001:0:175:214::/64 [115/20]
           via fe80::3e08:cdff:fe8d:badc, Ethernet5
 I L2     2001:0:175:217::/64 [115/20]
           via fe80::3e08:cdff:fe8d:badc, Ethernet5
 I L2     2002::30/128 [115/20]
           via fe80::c6ca:2bff:fe45:a215, Ethernet1
 I L2     2002::31/128 [115/30]
           via fe80::c6ca:2bff:fe45:a215, Ethernet1
 C        2002::32/128 [0/0]
           via Loopback0, directly connected
 I L2     2002::53/128 [115/20]
           via fe80::3e08:cdff:fe8d:badc, Ethernet5
 I L2     2002::175/128 [115/10]
           via fe80::3e08:cdff:fe8d:badc, Ethernet5

```

## show mpls route

```text
MPLS forwarding table (Label [metric] Vias) - 39 routes 
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
                    20.30.32.30 Ethernet1
 20031   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via IS-IS SR tunnel index 16
                    via 20.30.32.30, Ethernet1, label 20031
 20053   A[1]
                via M, ::, swap 10053
                    EgressACL: bypass
                  via IS-IS SR tunnel index 11
                    via 20.32.175.175, Ethernet5, label 20053
 20066   A[1]
                via M, forward
                    EgressACL: apply
                    20.32.175.175 Ethernet5
 20072   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via IS-IS SR tunnel index 4
                    via 20.30.32.30, Ethernet1, label 20072
 20084   A[1]
                via M, ::, swap 20084
                    EgressACL: bypass
                  via IS-IS SR tunnel index 3
                    via 20.30.32.30, Ethernet1, label 20084
 20120   A[1]
                via M, forward
                    EgressACL: apply
                    20.30.32.30 Ethernet1
 20122   A[1]
                via M, forward
                    EgressACL: apply
                    20.30.32.30 Ethernet1
 20128   A[1]
                via M, ::, swap 20128
                    EgressACL: bypass
                  via IS-IS SR tunnel index 10
                    via 20.32.175.175, Ethernet5, label 20128
 20157   A[1]
                via M, forward
                    EgressACL: apply
                    20.32.175.175 Ethernet5
 20175   A[1]
                via M, pop
                    EgressACL: apply
                    20.32.175.175 Ethernet5
 20179   A[1]
                via M, ::, swap 0
                    EgressACL: bypass
                  via IS-IS SR tunnel index 12
                    via 20.32.175.175, Ethernet5, label 20179
 20184   A[1]
                via M, ::, swap 20184
                    EgressACL: bypass
                  via IS-IS SR tunnel index 14
                    via 20.32.175.175, Ethernet5, label 20184
 20195   A[1]
                via M, forward
                    EgressACL: apply
                    20.32.175.175 Ethernet5
 20201    [0]
                via I, auto, vrf default
 20202    [0]
                via I, auto, vrf default
 20214   A[1]
                via M, forward
                    EgressACL: apply
                    20.32.175.175 Ethernet5
 20216   A[1]
                via M, ::, swap 20216
                    EgressACL: bypass
                  via IS-IS SR tunnel index 15
                    via 20.32.175.175, Ethernet5, label 20216
 20430   A[1]
                via M, pop
                    EgressACL: apply
                    fe80::c6ca:2bff:fe45:a215 Ethernet1
 20453   A[1]
                via M, forward
                    EgressACL: apply
                    fe80::3e08:cdff:fe8d:badc Ethernet5
 20575   A[1]
                via M, pop
                    EgressACL: apply
                    fe80::3e08:cdff:fe8d:badc Ethernet5
 21181   A[1]
                via M, forward
                    EgressACL: apply
                    20.32.175.175 Ethernet5
 21182   A[1]
                via M, forward
                    EgressACL: apply
                    20.32.175.175 Ethernet5
 21217   A[1]
                via M, forward
                    EgressACL: apply
                    20.32.175.175 Ethernet5
 21303   A[1]
                via M, pop
                    EgressACL: apply
                    20.32.175.175 Ethernet5
 21304   A[1]
                via M, pop
                    EgressACL: apply
                    20.32.175.175 Ethernet5
 21307   A[1]
                via M, forward
                    EgressACL: apply
                    20.32.175.175 Ethernet5
 21308   A[1]
                via M, forward
                    EgressACL: apply
                    20.32.175.175 Ethernet5
 21581   A[1]
                via M, forward
                    EgressACL: apply
                    fe80::3e08:cdff:fe8d:badc Ethernet5
 21582   A[1]
                via M, forward
                    EgressACL: apply
                    fe80::3e08:cdff:fe8d:badc Ethernet5
 21703   A[1]
                via M, pop
                    EgressACL: apply
                    fe80::3e08:cdff:fe8d:badc Ethernet5
 21704   A[1]
                via M, pop
                    EgressACL: apply
                    fe80::3e08:cdff:fe8d:badc Ethernet5
 362144  A[1]
                via M, 20.30.32.30, pop
                    EgressACL: apply
                    directly connected, Ethernet1
                    c4:ca:2b:45:a2:15, vlan 1006
 362145  A[1]
                via M, fe80::c6ca:2bff:fe45:a215, pop
                    EgressACL: apply
                    directly connected, Ethernet1
                    c4:ca:2b:45:a2:15, vlan 1006
 362146  A[1]
                via M, 20.32.175.175, pop
                    EgressACL: apply
                    directly connected, Ethernet5
                    3c:08:cd:8d:ba:dc, vlan 1010
 362147  A[1]
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
MPLS forwarding table (Label [metric] Vias) - 39 routes 
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
                via M, 20.30.32.30, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet1
 I>BL  20031    [1], 10.0.0.31/32
                via IS-IS SR tunnel index 16, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                    via 20.30.32.30, Ethernet1, label 20031
 I>BL  20053    [1], 10.0.0.53/32
                via IS-IS SR tunnel index 11, swap 10053
                 payload autoDecide, ttlMode uniform, apply egress-acl
                    via 20.32.175.175, Ethernet5, label 20053
 IP    20066    [1], 10.0.0.66/32
                via M, 20.32.175.175, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet5
 I>BL  20072    [1], 10.0.0.72/32
                via IS-IS SR tunnel index 4, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                    via 20.30.32.30, Ethernet1, label 20072
 I>BL  20084    [1], 10.0.0.84/32
                via IS-IS SR tunnel index 3, swap 20084
                 payload autoDecide, ttlMode uniform, apply egress-acl
                    via 20.30.32.30, Ethernet1, label 20084
 IP    20120    [1], 10.0.0.120/32
                via M, 20.30.32.30, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet1
 IP    20122    [1], 10.0.0.122/32
                via M, 20.30.32.30, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet1
 I>BL  20128    [1], 10.0.0.128/32
                via IS-IS SR tunnel index 10, swap 20128
                 payload autoDecide, ttlMode uniform, apply egress-acl
                    via 20.32.175.175, Ethernet5, label 20128
 IP    20157    [1], 10.0.0.157/32
                via M, 20.32.175.175, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet5
 IP    20175    [1], 10.0.0.175/32
                via M, 20.32.175.175, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet5
 I>BL  20179    [1], 10.0.0.179/32
                via IS-IS SR tunnel index 12, swap 0
                 payload autoDecide, ttlMode uniform, apply egress-acl
                    via 20.32.175.175, Ethernet5, label 20179
 I>BL  20184    [1], 10.0.0.184/32
                via IS-IS SR tunnel index 14, swap 20184
                 payload autoDecide, ttlMode uniform, apply egress-acl
                    via 20.32.175.175, Ethernet5, label 20184
 IP    20195    [1], 10.0.0.195/32
                via M, 20.32.175.175, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet5
 IP    20201    [0], 209.209.209.201/32
                via I, auto, vrf default
 IP    20202    [0], 209.209.209.202/32
                via I, auto, vrf default
 IP    20214    [1], 10.0.0.214/32
                via M, 20.32.175.175, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet5
 I>BL  20216    [1], 10.0.0.216/32
                via IS-IS SR tunnel index 15, swap 20216
                 payload autoDecide, ttlMode uniform, apply egress-acl
                    via 20.32.175.175, Ethernet5, label 20216
 IP    20430    [1], 2002::30/128
                via M, fe80::c6ca:2bff:fe45:a215, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet1
 IP    20453    [1], 2002::53/128
                via M, fe80::3e08:cdff:fe8d:badc, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet5
 IP    20575    [1], 2002::175/128
                via M, fe80::3e08:cdff:fe8d:badc, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet5
 IP    21181    [1], 10.0.0.53/32, algorithm MIN-LATENCY
                via M, 20.32.175.175, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet5
 IP    21182    [1], 10.0.0.53/32, algorithm MIN-TE
                via M, 20.32.175.175, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet5
 IP    21217    [1], 10.0.0.217/32
                via M, 20.32.175.175, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet5
 IP    21303    [1], 10.0.0.175/32, algorithm MIN-LATENCY
                via M, 20.32.175.175, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet5
 IP    21304    [1], 10.0.0.175/32, algorithm MIN-TE
                via M, 20.32.175.175, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet5
 IP    21307    [1], 10.0.0.179/32, algorithm MIN-LATENCY
                via M, 20.32.175.175, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet5
 IP    21308    [1], 10.0.0.179/32, algorithm MIN-TE
                via M, 20.32.175.175, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet5
 IP    21581    [1], 2002::53/128, algorithm MIN-LATENCY
                via M, fe80::3e08:cdff:fe8d:badc, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet5
 IP    21582    [1], 2002::53/128, algorithm MIN-TE
                via M, fe80::3e08:cdff:fe8d:badc, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet5
 IP    21703    [1], 2002::175/128, algorithm MIN-LATENCY
                via M, fe80::3e08:cdff:fe8d:badc, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet5
 IP    21704    [1], 2002::175/128, algorithm MIN-TE
                via M, fe80::3e08:cdff:fe8d:badc, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet5
 IA    362144   [1]
                via M, 20.30.32.30, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet1
 IA    362145   [1]
                via M, fe80::c6ca:2bff:fe45:a215, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet1
 IA    362146   [1]
                via M, 20.32.175.175, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet5
 IA    362147   [1]
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
 * >  L   10.0.0.31/32           10.0.0.31             0       -          125     0       i
 * >  L   10.0.0.53/32           10.0.0.53             0       -          100     0       ?
 * >  L   10.0.0.72/32           10.0.0.72             0       -          100     0       i
 * >  L   10.0.0.84/32           10.0.0.84             0       -          100     0       i
 * >  L   10.0.0.128/32          10.0.0.128            0       -          100     0       i
 * >  L   10.0.0.179/32          10.0.0.179            0       -          125     0       i
 * >  L   10.0.0.184/32          10.0.0.184            0       -          0       0       i
 * >  L   10.0.0.216/32          10.0.0.216            0       -          100     0       i
```

## show bgp neighbors

```text
BGP neighbor is 10.0.0.30, remote AS 64512, internal link
 Description: Arista-Spine30
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
  Outbound route map for VPN-IPv6 is SET_COLOR_101
Local AS is 64512, local router ID 10.0.0.32
TTL is 255

BGP neighbor is 10.0.0.31, remote AS 65001, internal link
 Description: ARISTA-LU-RIGHT-PEERING
  BGP version 4, remote router ID 10.0.0.31, VRF default
  Inherits configuration from and member of peer-group IBGP-RIGHT-LU
  Last read 00:00:01, last write 00:00:26
  Hold time is 180, keepalive interval is 60 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:02:59
  Keepalive timer is active, time left: 00:00:17
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 00:39:07
  Number of transitions to established: 3
  Last state was OpenConfirm
  Last event was ReapplyOutboundPolicy
  Last rcvd notification:Cease/administrative reset, Last time 00:39:08, First time 12:37:35, Repeats 1
  Last sent socket-error:Connect (Network is unreachable), Last time 17:27:39, First time 20:04:56, Repeats 62
  Types of communities advertised: standard extended large
  Enhanced route refresh stale path removal disabled
  Outbound enhanced route refresh enabled
  Neighbor is a route reflector client
  Neighbor is using cluster ID 32.32.32.201
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
      Restart-State bit: no
      Graceful notification: yes
      IPv4 with MPLS Labels is enabled, Forwarding State is not preserved
    Graceful Restart received:
      Restart-time is 120
      Restart-State bit: yes
      Graceful notification: yes
      IPv4 with MPLS Labels is enabled, Forwarding State is not preserved
    Multiple labels capability:
      IPv4 with MPLS Labels: advertised with count 13
      IPv4 with MPLS Labels: received with count 13
  Restart timer is inactive
  End of rib timer is inactive
    IPv4 with MPLS Labels End-of-RIB received: Yes
      Received 00:38:16
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
    Opens:                           3         3
    Notifications:                   0         2
    Updates:                        60        14
    Keepalives:                   1210      1230
    Enhanced Route Refresh:          0         0
    Begin of Route Refresh:          0         0
    End of Route Refresh:            0         0
    Total messages:               1273      1249
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    IPv4 with MPLS Labels:            7         1              1                   0
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
Local AS is 65001, local router ID 10.0.0.32
TTL is 255
Local TCP address is 10.0.0.32, local port is 34073
Remote TCP address is 10.0.0.31, remote port is 179
Local next hop for next hop self:
  IPv4 with MPLS Labels: 209.209.209.202
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
    TCP Throughput: 538.79 Mbps
    Advertised Recv Window (rcv_space): 14480

BGP neighbor is 10.0.0.53, remote AS 65000, internal link
 Description: Arccus_53
  BGP version 4, remote router ID 10.0.0.53, VRF default
  Inherits configuration from and member of peer-group IBGP-LEFT-LU
  Last read 00:00:28, last write 00:00:30
  Hold time is 180, keepalive interval is 60 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:02:32
  Keepalive timer is active, time left: 00:00:25
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 16:00:27
  Number of transitions to established: 3
  Last state was OpenConfirm
  Last event was RecvUpdate
  Last rcvd notification:Cease/administrative reset, Last time 16:00:28, First time 16:02:31, Repeats 1
  Last rcvd socket-error:Connection reset by peer, Last time 16:27:07, First time 16:28:52, Repeats 6
  Types of communities advertised: standard extended large
  Neighbor is a route reflector client
  Neighbor is using cluster ID 32.32.32.201
  Neighbor Capabilities:
    Multiprotocol IPv4 Unicast: received
    Multiprotocol IPv4 with MPLS Labels: advertised and received and negotiated
    Four Octet ASN: advertised and received and negotiated
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
      Restart-time is 120
      Restart-State bit: no
      Graceful notification: no
      IPv4 Unicast is enabled, Forwarding State is preserved
      IPv4 with MPLS Labels is enabled, Forwarding State is preserved
    Multiple labels capability:
      IPv4 with MPLS Labels: advertised with count 13
  Restart timer is inactive
  End of rib timer is inactive
    IPv4 with MPLS Labels End-of-RIB received: Yes
      Received 16:00:27
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
    Opens:                 10         3
    Notifications:          0         2
    Updates:               52        10
    Keepalives:          1153       988
    Route Refresh:          0         0
    Total messages:      1215      1003
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    IPv4 with MPLS Labels:            7         1              1                   0
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
Local AS is 65000, local router ID 10.0.0.32
TTL is 255
Local TCP address is 10.0.0.32, local port is 36887
Remote TCP address is 10.0.0.53, remote port is 179
Local next hop for next hop self:
  IPv4 with MPLS Labels: 209.209.209.201
TCP Socket Information:
  TCP state is ESTABLISHED
  Recv-Q: 0/32768
  Send-Q: 0/46080
  Outgoing Maximum Segment Size (MSS): 1432
  Total Number of TCP retransmissions: 0
  Options:
    Timestamps enabled: yes
    Selective Acknowledgments enabled: yes
    Window Scale enabled: yes
    Explicit Congestion Notification (ECN) enabled: no
  Socket Statistics:
    Window Scale (wscale): 14,7
    Retransmission Timeout (rto): 204.0ms
    Round-trip Time (rtt/rtvar): 0.3ms/0.0ms
    Delayed Ack Timeout (ato): 40.0ms
    Congestion Window (cwnd): 10
    TCP Throughput: 442.32 Mbps
    Advertised Recv Window (rcv_space): 14480

BGP neighbor is 10.0.0.54, remote AS 65000, internal link
 Description: ARRCUS-LU-LEFT-PEERING
  BGP version 4, remote router ID 0.0.0.0, VRF default
  Inherits configuration from and member of peer-group IBGP-LEFT-LU
  Last read never, last write 18:44:19
  Hold time is 0, keepalive interval is 0 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is inactive
  Keepalive timer is inactive
  Connect timer is active, time left: 00:01:11
  Connection interval is 148 seconds
  Failed connection attempts is 404
  Idle-restart timer is inactive
  BGP state is Active
  Number of transitions to established: 0
  Last state was Connect
  Last event was TransportError
  Last sent socket-error:Connect (Network is unreachable), Last time 00:01:19, First time 20:07:36, Repeats 436
  Last rcvd socket-error:Connection reset by peer, Last time 18:44:19, First time 18:44:28, Repeats 2
  Types of communities advertised: standard extended large
  Neighbor is a route reflector client
  Neighbor is using cluster ID 32.32.32.201
  Neighbor Capabilities:
    Multiprotocol IPv4 with MPLS Labels: advertised
    Four Octet ASN: advertised
    Route Refresh: advertised
    Enhanced route refresh: advertised
    Send End-of-RIB messages: advertised
    Additional-paths recv capability:
      IPv4 with MPLS Labels: advertised
    Additional-paths send capability:
    Graceful Restart advertised:
      Restart-time is 120
      Restart-State bit: no
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
    Opens:                  3         0
    Notifications:          0         0
    Updates:                0         0
    Keepalives:             0         0
    Route Refresh:          0         0
    Total messages:         3         0
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
Local AS is 65000, local router ID 10.0.0.32
TTL is 255
Local TCP address is 10.0.0.32
Remote TCP address is 10.0.0.54, remote port is 179

BGP neighbor is 10.0.0.72, remote AS 65001, internal link
 Description: CIENA-LU-RIGHT-PEERING
  BGP version 4, remote router ID 10.0.0.72, VRF default
  Inherits configuration from and member of peer-group IBGP-RIGHT-LU
  Last read 00:00:41, last write 00:00:10
  Hold time is 180, keepalive interval is 60 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:02:19
  Keepalive timer is active, time left: 00:00:39
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 15:51:41
  Number of transitions to established: 14
  Last state was OpenConfirm
  Last event was ReapplyOutboundPolicy
  Last sent notification:Open Message Error/unsupported capability, Last time 18:03:09, First time 18:06:06, Repeats 35
    Sent data: 0x010400010004
  Last rcvd notification:Cease/peer de-configured, Last time 15:52:17, First time 16:39:40, Repeats 6
  Last sent socket-error:Connect (Connection refused), Last time 15:51:53, First time 17:43:26, Repeats 48
  Last rcvd socket-error:Connection reset by peer, Last time 15:59:02, First time 18:44:30, Repeats 19
  Types of communities advertised: standard extended large
  Neighbor is a route reflector client
  Neighbor is using cluster ID 32.32.32.201
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
      Received 15:51:31
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
    Opens:                 70        50
    Notifications:         36        13
    Updates:              136        65
    Keepalives:          1221      1047
    Route Refresh:          0         7
    Total messages:      1463      1182
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    IPv4 with MPLS Labels:            7         1              1                   0
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
Local AS is 65001, local router ID 10.0.0.32
TTL is 255
Local TCP address is 10.0.0.32, local port is 179
Remote TCP address is 10.0.0.72, remote port is 43251
Local next hop for next hop self:
  IPv4 with MPLS Labels: 209.209.209.202
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
    TCP Throughput: 183.07 Mbps
    Advertised Recv Window (rcv_space): 14600

BGP neighbor is 10.0.0.84, remote AS 65001, internal link
 Description: ERICSSON-LU-RIGHT-PEERING
  BGP version 4, remote router ID 10.0.0.84, VRF default
  Inherits configuration from and member of peer-group IBGP-RIGHT-LU
  Last read 00:00:07, last write 00:00:04
  Hold time is 90, keepalive interval is 30 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:01:23
  Keepalive timer is active, time left: 00:00:16
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 16:51:02
  Number of transitions to established: 1
  Last state was OpenConfirm
  Last event was ReapplyOutboundPolicy
  Last sent socket-error:Connect (Network is unreachable), Last time 17:45:12
  Types of communities advertised: standard extended large
  Enhanced route refresh stale path removal disabled
  Outbound enhanced route refresh enabled
  Neighbor is a route reflector client
  Neighbor is using cluster ID 32.32.32.201
  Neighbor Capabilities:
    Multiprotocol IPv4 Unicast: received
    Multiprotocol IPv4 with MPLS Labels: advertised and received and negotiated
    Four Octet ASN: advertised and received and negotiated
    Route Refresh: advertised and received and negotiated
    Enhanced route refresh: advertised and received and negotiated
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
      Restart-time is 120
      Restart-State bit: no
      Graceful notification: no
      IPv4 Unicast is enabled, Forwarding State is preserved
      IPv4 with MPLS Labels is enabled, Forwarding State is preserved
    Multiple labels capability:
      IPv4 with MPLS Labels: advertised with count 13
  Restart timer is inactive
  End of rib timer is inactive
    IPv4 with MPLS Labels End-of-RIB received: Yes
      Received 16:51:02
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
    Updates:                        54         2
    Keepalives:                   2354      2017
    Enhanced Route Refresh:          0         0
    Begin of Route Refresh:          0         0
    End of Route Refresh:            0         0
    Total messages:               2409      2020
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    IPv4 with MPLS Labels:            7         1              1                   0
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
Local AS is 65001, local router ID 10.0.0.32
TTL is 255
Local TCP address is 10.0.0.32, local port is 36105
Remote TCP address is 10.0.0.84, remote port is 179
Local next hop for next hop self:
  IPv4 with MPLS Labels: 209.209.209.202
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
    Round-trip Time (rtt/rtvar): 231.1ms/1.4ms
    Delayed Ack Timeout (ato): 40.0ms
    Congestion Window (cwnd): 10
    TCP Throughput: 0.49 Mbps
    Advertised Recv Window (rcv_space): 14480

BGP neighbor is 10.0.0.122, remote AS 65001, internal link
 Description: H3C-LU-RIGHT-PEERING
  BGP version 4, remote router ID 10.0.0.122, VRF default
  Inherits configuration from and member of peer-group IBGP-RIGHT-LU
  Last read 00:00:16, last write 00:00:56
  Hold time is 180, keepalive interval is 60 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:02:44
  Keepalive timer is active, time left: 00:00:02
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 00:29:22
  Number of transitions to established: 1
  Last state was OpenConfirm
  Last event was ReapplyOutboundPolicy
  Types of communities advertised: standard extended large
  Neighbor is a route reflector client
  Neighbor is using cluster ID 32.32.32.201
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
      Restart-State bit: no
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
    Opens:                  1         1
    Notifications:          0         0
    Updates:               12         1
    Keepalives:            36        31
    Route Refresh:          0         0
    Total messages:        49        33
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    IPv4 with MPLS Labels:            8         0              0                   0
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
Local AS is 65001, local router ID 10.0.0.32
TTL is 255
Local TCP address is 10.0.0.32, local port is 35037
Remote TCP address is 10.0.0.122, remote port is 179
Local next hop for next hop self:
  IPv4 with MPLS Labels: 209.209.209.202
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
    TCP Throughput: 180.92 Mbps
    Advertised Recv Window (rcv_space): 14480

BGP neighbor is 10.0.0.128, remote AS 65000, internal link
 Description: HUAWEI-LU-LEFT-PEERING
  BGP version 4, remote router ID 10.0.0.128, VRF default
  Inherits configuration from and member of peer-group IBGP-LEFT-LU
  Last read 00:00:47, last write 00:00:24
  Hold time is 180, keepalive interval is 60 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:02:13
  Keepalive timer is active, time left: 00:00:34
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 01:59:47
  Number of transitions to established: 1
  Last state was OpenConfirm
  Last event was Open
  Last sent notification:Cease/connection collision resolution, Last time 00:00:06, First time 01:11:46, Repeats 107
  Last sent socket-error:Connect (Connection refused), Last time 02:03:29, First time 17:42:37, Repeats 336
  Last rcvd socket-error:Connection reset by peer, Last time 02:00:56
  Types of communities advertised: standard extended large
  Neighbor is a route reflector client
  Neighbor is using cluster ID 32.32.32.201
  Neighbor Capabilities:
    Multiprotocol IPv4 Unicast: received
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
      Restart-State bit: no
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
    Opens:                  4       111
    Notifications:        110         0
    Updates:               21         7
    Keepalives:           136       140
    Route Refresh:          0         0
    Total messages:       271       258
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    IPv4 with MPLS Labels:            7         1              1                   0
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
Local AS is 65000, local router ID 10.0.0.32
TTL is 255
Local TCP address is 10.0.0.32, local port is 179
Remote TCP address is 10.0.0.128, remote port is 58226
Local next hop for next hop self:
  IPv4 with MPLS Labels: 209.209.209.201
TCP Socket Information:
  TCP state is ESTABLISHED
  Recv-Q: 0/32768
  Send-Q: 0/46080
  Outgoing Maximum Segment Size (MSS): 1460
  Total Number of TCP retransmissions: 0
  Options:
    Timestamps enabled: no
    Selective Acknowledgments enabled: no
    Window Scale enabled: no
    Explicit Congestion Notification (ECN) enabled: no
  Socket Statistics:
    Window Scale (wscale): 0,0
    Retransmission Timeout (rto): 360.0ms
    Round-trip Time (rtt/rtvar): 154.2ms/37.8ms
    Delayed Ack Timeout (ato): 40.0ms
    Congestion Window (cwnd): 10
    TCP Throughput: 0.76 Mbps
    Advertised Recv Window (rcv_space): 14600

BGP neighbor is 10.0.0.175, remote AS 64512, internal link
 Description: Juniper_175
  BGP version 4, remote router ID 10.0.0.175, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 18:11:58, last write 18:11:58
  Hold time is 90, keepalive interval is 30 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is inactive
  Keepalive timer is inactive
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Idle, Peer is not activated in any address-family mode
  Peering failure hint: Peer is not activated in any address-family mode
  Number of transitions to established: 138
  Last state was Active
  Last event was Stop
  Last sent notification:Open Message Error/unsupported capability, Last time 18:11:58, First time 6d16h, Repeats 13
    Sent data: 0x010400010080010400020080
  Last rcvd notification:Cease/peer de-configured, Last time 18:19:55
  Last sent socket-error:Connect (Network is unreachable), Last time 6d16h, First time 7d23h, Repeats 64
  Last rcvd socket-error:Connection reset by peer, Last time 7d23h
  Types of communities advertised: standard extended large
  Neighbor Capabilities:
    Multiprotocol VPN-IPv4: advertised
    Multiprotocol VPN-IPv6: advertised
    Four Octet ASN: advertised
    Route Refresh: advertised
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
    Opens:                152       152
    Notifications:         25       126
    Updates:              971      2103
    Keepalives:         30369     27516
    Route Refresh:          0         0
    Total messages:     31517     29897
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
  Outbound route map for VPN-IPv6 is SET_COLOR_101
Local AS is 64512, local router ID 10.0.0.32
TTL is 255
Remote TCP address is 10.0.0.175

BGP neighbor is 10.0.0.179, remote AS 65000, internal link
 Description: JUNIPER-LU-LEFT-PEERING
  BGP version 4, remote router ID 10.0.0.179, VRF default
  Inherits configuration from and member of peer-group IBGP-LEFT-LU
  Last read 00:00:01, last write 00:00:22
  Hold time is 90, keepalive interval is 30 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:01:29
  Keepalive timer is active, time left: 00:00:06
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 00:40:49
  Number of transitions to established: 3
  Last state was OpenConfirm
  Last event was RecvUpdate
  Last sent notification:Hold Timer Expired Error/None, Last time 17:42:35
  Last rcvd notification:Cease/peer de-configured, Last time 00:40:50
  Last sent socket-error:Connect (Network is unreachable), Last time 18:06:55, First time 18:35:12, Repeats 7
  Types of communities advertised: standard extended large
  Neighbor is a route reflector client
  Neighbor is using cluster ID 32.32.32.201
  Neighbor Capabilities:
    Multiprotocol IPv4 with MPLS Labels: advertised and received and negotiated
    Four Octet ASN: advertised and received and negotiated
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
      Restart-time is 120
      Restart-State bit: no
      Graceful notification: yes
    Long Lived Graceful Restart received:
      Helper only
    Multiple labels capability:
      IPv4 with MPLS Labels: advertised with count 13
  Restart timer is inactive
  End of rib timer is inactive
    IPv4 with MPLS Labels End-of-RIB received: Yes
      Received 00:40:49
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
    Opens:                 61        62
    Notifications:         60         1
    Updates:               59         6
    Keepalives:          2506      2355
    Route Refresh:          0         0
    Total messages:      2686      2424
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    IPv4 with MPLS Labels:            7         1              1                   0
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
Local AS is 65000, local router ID 10.0.0.32
TTL is 255
Local TCP address is 10.0.0.32, local port is 43819
Remote TCP address is 10.0.0.179, remote port is 179
Local next hop for next hop self:
  IPv4 with MPLS Labels: 209.209.209.201
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
    Round-trip Time (rtt/rtvar): 0.7ms/0.1ms
    Delayed Ack Timeout (ato): 40.0ms
    Congestion Window (cwnd): 10
    TCP Throughput: 155.49 Mbps
    Advertised Recv Window (rcv_space): 14480

BGP neighbor is 10.0.0.184, remote AS 65000, internal link
 Description: KEYSIGHT-LU-LEFT-PEERING
  BGP version 4, remote router ID 192.0.0.1, VRF default
  Inherits configuration from and member of peer-group IBGP-LEFT-LU
  Last read 00:00:03, last write 00:00:01
  Hold time is 90, keepalive interval is 30 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:01:27
  Keepalive timer is active, time left: 00:00:26
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 00:22:03
  Number of transitions to established: 3
  Last state was OpenConfirm
  Last event was RecvUpdate
  Last sent socket-error:Connect (Network is unreachable), Last time 01:38:23, First time 20:07:36, Repeats 367
  Last rcvd socket-error:Connection reset by peer, Last time 00:24:42, First time 19:48:49, Repeats 138
  Types of communities advertised: standard extended large
  Neighbor is a route reflector client
  Neighbor is using cluster ID 32.32.32.201
  Neighbor Capabilities:
    Multiprotocol IPv4 Unicast: received
    Multiprotocol IPv4 Multicast: received
    Multiprotocol IPv4 with MPLS Labels: advertised and received and negotiated
    Multiprotocol VPN-IPv4: received
    Four Octet ASN: advertised
    Route Refresh: advertised and received and negotiated
    Enhanced route refresh: advertised
    Send End-of-RIB messages: advertised
    Additional-paths recv capability:
      IPv4 with MPLS Labels: advertised
    Additional-paths send capability:
    Graceful Restart advertised:
      Restart-time is 120
      Restart-State bit: no
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
    Opens:                140         3
    Notifications:          0         0
    Updates:               21         3
    Keepalives:            62        55
    Route Refresh:          0         0
    Total messages:       223        61
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    IPv4 with MPLS Labels:            7         1              1                   0
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
Local AS is 65000, local router ID 10.0.0.32
TTL is 255
Local TCP address is 10.0.0.32, local port is 179
Remote TCP address is 10.0.0.184, remote port is 33395
Local next hop for next hop self:
  IPv4 with MPLS Labels: 209.209.209.201
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
    Round-trip Time (rtt/rtvar): 0.2ms/0.0ms
    Delayed Ack Timeout (ato): 40.0ms
    Congestion Window (cwnd): 10
    TCP Throughput: 609.68 Mbps
    Advertised Recv Window (rcv_space): 14600

BGP neighbor is 10.0.0.216, remote AS 65000, internal link
 Description: NOKIA-LU-LEFT-PEERING
  BGP version 4, remote router ID 10.0.0.216, VRF default
  Inherits configuration from and member of peer-group IBGP-LEFT-LU
  Last read 00:00:12, last write 00:00:02
  Hold time is 90, keepalive interval is 30 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:01:18
  Keepalive timer is active, time left: 00:00:23
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 15:26:14
  Number of transitions to established: 5
  Last state was OpenConfirm
  Last event was RecvUpdate
  Last sent notification:Hold Timer Expired Error/None, Last time 17:42:21
  Last rcvd notification:Cease/administrative shutdown, Last time 15:26:45, First time 19:46:50, Repeats 2
  Last rcvd socket-error:Connection reset by peer, Last time 15:26:20, First time 20:07:35, Repeats 14
  Types of communities advertised: standard extended large
  Neighbor is a route reflector client
  Neighbor is using cluster ID 32.32.32.201
  Neighbor Capabilities:
    Multiprotocol IPv4 with MPLS Labels: advertised and received and negotiated
    Four Octet ASN: advertised and received and negotiated
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
      Restart-time is 120
      Restart-State bit: no
      Graceful notification: no
    Multiple labels capability:
      IPv4 with MPLS Labels: advertised with count 13
  Restart timer is inactive
  End of rib timer is inactive
    IPv4 with MPLS Labels End-of-RIB received: Yes
      Received 15:26:13
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
    Opens:                 20         6
    Notifications:          2         3
    Updates:               59        17
    Keepalives:          2811      2415
    Route Refresh:          0         0
    Total messages:      2892      2441
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    IPv4 with MPLS Labels:            7         1              1                   0
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
Local AS is 65000, local router ID 10.0.0.32
TTL is 255
Local TCP address is 10.0.0.32, local port is 179
Remote TCP address is 10.0.0.216, remote port is 57200
Local next hop for next hop self:
  IPv4 with MPLS Labels: 209.209.209.201
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
    Round-trip Time (rtt/rtvar): 0.8ms/0.0ms
    Delayed Ack Timeout (ato): 40.0ms
    Congestion Window (cwnd): 10
    TCP Throughput: 104.46 Mbps
    Advertised Recv Window (rcv_space): 14600

```

## show bgp labeled-unicast tunnel

```text
Index  Endpoint       Nexthop/Tunnel Index  Interface  Labels     Contributing 
------ -------------- --------------------- ---------- ---------- -------------
9      10.0.0.84/32   IS-IS SR IPv4 (3)     -          [ 20084 ]  Yes          
20     10.0.0.53/32   IS-IS SR IPv4 (11)    -          [ 10053 ]  Yes          
22     10.0.0.216/32  IS-IS SR IPv4 (15)    -          [ 20216 ]  Yes          
24     10.0.0.72/32   IS-IS SR IPv4 (4)     -          [ 3 ]      Yes          
25     10.0.0.128/32  IS-IS SR IPv4 (10)    -          [ 20128 ]  Yes          
29     10.0.0.179/32  IS-IS SR IPv4 (12)    -          [ 0 ]      Yes          
30     10.0.0.31/32   IS-IS SR IPv4 (16)    -          [ 3 ]      Yes          
31     10.0.0.184/32  IS-IS SR IPv4 (14)    -          [ 20184 ]  Yes          

   Metric/Type       Metric 2       Pref    Pref 2
----------------- -------------- ---------- ------
      0 MED          0              200     0     
      0 MED          0              200     0     
      0 MED          0              200     0     
      0 MED          0              200     0     
      0 MED          0              200     0     
      0 MED          0              200     0     
      0 MED          0              200     0     
      0 MED          0              200     0     

```

## show bgp labeled-unicast forwarding

```text
   Index       Nexthop                  Interface    Labels   
----------- ------------------------ --------------- ---------
   19          IS-IS SR IPv4 (3)        -            [ 20084 ]
   20          IS-IS SR IPv4 (3)        -            [ 20084 ]
   45          IS-IS SR IPv4 (15)       -            [ 20216 ]
   46          IS-IS SR IPv4 (15)       -            [ 20216 ]
   47          IS-IS SR IPv4 (11)       -            [ 10053 ]
   48          IS-IS SR IPv4 (11)       -            [ 10053 ]
   51          IS-IS SR IPv4 (4)        -            [ 3 ]    
   52          IS-IS SR IPv4 (4)        -            [ 3 ]    
   53          IS-IS SR IPv4 (10)       -            [ 20128 ]
   54          IS-IS SR IPv4 (10)       -            [ 20128 ]
   63          IS-IS SR IPv4 (12)       -            [ 0 ]    
   64          IS-IS SR IPv4 (12)       -            [ 0 ]    
   65          IS-IS SR IPv4 (16)       -            [ 3 ]    
   66          IS-IS SR IPv4 (16)       -            [ 3 ]    
   67          IS-IS SR IPv4 (14)       -            [ 20184 ]
   68          IS-IS SR IPv4 (14)       -            [ 20184 ]

```

## show tunnel rib system-tunnel-rib brief

```text
Tunnel RIB: system-tunnel-rib
Endpoint        Tunnel Type     Index(es)   Tunnel Preference   IGP Preference 
-------------- --------------- ----------- ------------------- ----------------
10.0.0.30/32    IS-IS SR IPv4   1           10                  115            
10.0.0.31/32    IS-IS SR IPv4   16          10                  115            
10.0.0.53/32    IS-IS SR IPv4   11          10                  115            
10.0.0.66/32    IS-IS SR IPv4   22          10                  115            
10.0.0.72/32    IS-IS SR IPv4   4           10                  115            
10.0.0.84/32    IS-IS SR IPv4   3           10                  115            
10.0.0.120/32   IS-IS SR IPv4   17          10                  115            
10.0.0.122/32   IS-IS SR IPv4   21          10                  115            
10.0.0.128/32   IS-IS SR IPv4   10          10                  115            
10.0.0.157/32   IS-IS SR IPv4   18          10                  115            
10.0.0.175/32   IS-IS SR IPv4   5           10                  115            
10.0.0.179/32   IS-IS SR IPv4   12          10                  115            
10.0.0.184/32   IS-IS SR IPv4   14          10                  115            
10.0.0.195/32   IS-IS SR IPv4   19          10                  115            
10.0.0.214/32   IS-IS SR IPv4   7           10                  115            
10.0.0.216/32   IS-IS SR IPv4   15          10                  115            
10.0.0.217/32   IS-IS SR IPv4   20          10                  115            
2002::175/128   IS-IS SR IPv6   9           10                  115            
2002::30/128    IS-IS SR IPv6   2           10                  115            
2002::53/128    IS-IS SR IPv6   13          10                  115            

   IGP Metric    Metric Type
---------------- -----------
   10            metric     
   85            metric     
   110           metric     
   110           metric     
   120           metric     
   120           metric     
   110           metric     
   110           metric     
   110           metric     
   120           metric     
   10            metric     
   110           metric     
   120           metric     
   140           metric     
   85            metric     
   110           metric     
   120           metric     
   10            metric     
   20            metric     
   20            metric     

```

## show tunnel rib colored brief

```text
Tunnel RIB: system-colored-tunnel-rib
 Endpoint        Color   Tunnel Type       Index(es)    Tunnel Preference    IGP Preference    IGP Metric   Metric Type
--------------- ------- ----------------- ------------ -------------------- ----------------- ------------- -----------
 10.0.0.53/32    128     IS-IS FlexAlgo    6            65                   115               200000       metric     
 10.0.0.53/32    129     IS-IS FlexAlgo    5            65                   115               20           metric     
 10.0.0.175/32   128     IS-IS FlexAlgo    2            65                   115               100000       metric     
 10.0.0.175/32   129     IS-IS FlexAlgo    1            65                   115               10           metric     
 10.0.0.179/32   128     IS-IS FlexAlgo    8            65                   115               200000       metric     
 10.0.0.179/32   129     IS-IS FlexAlgo    7            65                   115               20           metric     
 2002::53/128    128     IS-IS FlexAlgo    10           65                   115               200000       metric     
 2002::53/128    129     IS-IS FlexAlgo    9            65                   115               20           metric     
 2002::175/128   128     IS-IS FlexAlgo    4            65                   115               100000       metric     
 2002::175/128   129     IS-IS FlexAlgo    3            65                   115               10           metric     

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
>C    10.0.0.32/32 [0 pref/0 metric] updated 9d20h ago
         via Loopback0, directly connected
>C    20.30.32.0/24 [0 pref/0 metric] updated 18:04:52 ago
         via Ethernet1, directly connected
>C    20.32.175.0/24 [0 pref/0 metric] updated 5d19h ago
         via Ethernet5, directly connected
>C    209.209.209.201/32 [0 pref/0 metric] updated 20:14:21 ago
         via Loopback201, directly connected
>C    209.209.209.202/32 [0 pref/0 metric] updated 20:14:15 ago
         via Loopback202, directly connected
VRF: default, Protocol: bgp
Codes: C - Connected, S - Static, P - Route Input, G - Gribi
       B - BGP, O - Ospf, O3 - Ospf3, I - Isis, R - Rip, VL - VRF Leak
       > - Best Route, * - Unresolved Next hop
       EM - Exact match of the SR-TE Policy
       NM - Null endpoint match of the SR-TE Policy
       AM - Any endpoint match of the SR-TE Policy
       L - Part of a recursive route resolution loop
       A - Next hop not resolved in ARP/ND
       NF - Not in FEC
 B    10.0.0.31/32 [200 pref/0 MED] updated 00:37:31 ago
         via BGP LU Forwarding IPv4 Tunnel index 66
            via IS-IS SR Tunnel index 16 label 3
               via ::, NextLevelFecId2493952.714 label 20031 [NF]
 B    10.0.0.53/32 [200 pref/0 MED] updated 15:04:58 ago
         via BGP LU Forwarding IPv4 Tunnel index 48
            via IS-IS SR Tunnel index 11 label 10053
               via ::, NextLevelFecId2493952.716 label 20053 [NF]
 B    10.0.0.72/32 [200 pref/0 MED] updated 04:03:33 ago
         via BGP LU Forwarding IPv4 Tunnel index 52
            via IS-IS SR Tunnel index 4 label 3
               via ::, NextLevelFecId2493952.714 label 20072 [NF]
 B    10.0.0.84/32 [200 pref/0 MED] updated 16:51:03 ago
         via BGP LU Forwarding IPv4 Tunnel index 20
            via IS-IS SR Tunnel index 3 label 20084
               via ::, NextLevelFecId2493952.714 label 20084 [NF]
 B    10.0.0.128/32 [200 pref/0 MED] updated 01:59:48 ago
         via BGP LU Forwarding IPv4 Tunnel index 54
            via IS-IS SR Tunnel index 10 label 20128
               via ::, NextLevelFecId2493952.716 label 20128 [NF]
 B    10.0.0.179/32 [200 pref/0 MED] updated 00:40:49 ago
         via BGP LU Forwarding IPv4 Tunnel index 64
            via IS-IS SR Tunnel index 12 label 0
               via ::, NextLevelFecId2493952.716 label 20179 [NF]
 B    10.0.0.184/32 [200 pref/0 MED] updated 00:22:04 ago
         via BGP LU Forwarding IPv4 Tunnel index 68
            via IS-IS SR Tunnel index 14 label 20184
               via ::, NextLevelFecId2493952.716 label 20184 [NF]
 B    10.0.0.216/32 [200 pref/0 MED] updated 15:26:14 ago
         via BGP LU Forwarding IPv4 Tunnel index 46
            via IS-IS SR Tunnel index 15 label 20216
               via ::, NextLevelFecId2493952.716 label 20216 [NF]
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
>I    10.0.0.30/32 [115 pref/10 metric] updated 17:44:04 ago
         via 20.30.32.30, Ethernet1
>I    10.0.0.31/32 [115 pref/85 metric] updated 00:29:47 ago
         via 20.30.32.30, Ethernet1
>I    10.0.0.53/32 [115 pref/110 metric] updated 01:11:51 ago
         via 20.32.175.175, Ethernet5
>I    10.0.0.66/32 [115 pref/110 metric] updated 01:11:51 ago
         via 20.30.32.30, Ethernet1
>I    10.0.0.72/32 [115 pref/120 metric] updated 01:04:34 ago
         via 20.30.32.30, Ethernet1
>I    10.0.0.84/32 [115 pref/120 metric] updated 01:04:34 ago
         via 20.30.32.30, Ethernet1
>I    10.0.0.120/32 [115 pref/110 metric] updated 01:11:51 ago
         via 20.30.32.30, Ethernet1
>I    10.0.0.122/32 [115 pref/110 metric] updated 01:11:51 ago
         via 20.30.32.30, Ethernet1
>I    10.0.0.128/32 [115 pref/110 metric] updated 01:11:51 ago
         via 20.32.175.175, Ethernet5
>I    10.0.0.157/32 [115 pref/120 metric] updated 01:11:51 ago
         via 20.32.175.175, Ethernet5
>I    10.0.0.175/32 [115 pref/10 metric] updated 17:42:49 ago
         via 20.32.175.175, Ethernet5
>I    10.0.0.179/32 [115 pref/110 metric] updated 01:11:51 ago
         via 20.32.175.175, Ethernet5
>I    10.0.0.184/32 [115 pref/120 metric] updated 01:11:51 ago
         via 20.32.175.175, Ethernet5
>I    10.0.0.195/32 [115 pref/140 metric] updated 01:11:51 ago
         via 20.32.175.175, Ethernet5
>I    10.0.0.214/32 [115 pref/85 metric] updated 00:41:29 ago
         via 20.32.175.175, Ethernet5
>I    10.0.0.216/32 [115 pref/110 metric] updated 01:11:51 ago
         via 20.32.175.175, Ethernet5
>I    10.0.0.217/32 [115 pref/120 metric] updated 01:11:51 ago
         via 20.32.175.175, Ethernet5
>I    20.30.31.0/24 [115 pref/85 metric] updated 00:29:47 ago
         via 20.30.32.30, Ethernet1
>I    20.30.66.0/24 [115 pref/110 metric] updated 01:11:51 ago
         via 20.30.32.30, Ethernet1
>I    20.30.72.0/24 [115 pref/110 metric] updated 01:11:51 ago
         via 20.30.32.30, Ethernet1
>I    20.30.84.0/24 [115 pref/110 metric] updated 01:11:51 ago
         via 20.30.32.30, Ethernet1
>I    20.30.120.0/24 [115 pref/110 metric] updated 01:11:51 ago
         via 20.30.32.30, Ethernet1
>I    20.30.122.0/24 [115 pref/110 metric] updated 01:11:51 ago
         via 20.30.32.30, Ethernet1
>I    20.30.214.0/24 [115 pref/110 metric] updated 01:11:51 ago
         via 20.30.32.30, Ethernet1
>I    20.53.66.0/24 [115 pref/120 metric] updated 01:11:51 ago
         via 20.32.175.175, Ethernet5
>I    20.53.72.0/24 [115 pref/120 metric] updated 01:11:51 ago
         via 20.32.175.175, Ethernet5
>I    20.53.120.0/24 [115 pref/120 metric] updated 01:11:51 ago
         via 20.32.175.175, Ethernet5
>I    20.53.175.0/24 [115 pref/110 metric] updated 01:11:51 ago
         via 20.32.175.175, Ethernet5
>I    20.66.175.0/24 [115 pref/110 metric] updated 01:11:51 ago
         via 20.32.175.175, Ethernet5
>I    20.72.175.0/24 [115 pref/20 metric] updated 17:42:49 ago
         via 20.32.175.175, Ethernet5
>I    20.120.175.0/24 [115 pref/110 metric] updated 01:11:51 ago
         via 20.32.175.175, Ethernet5
>I    20.128.157.0/24 [115 pref/120 metric] updated 01:11:51 ago
         via 20.32.175.175, Ethernet5
>I    20.128.175.0/24 [115 pref/110 metric] updated 01:11:51 ago
         via 20.32.175.175, Ethernet5
>I    20.128.217.0/24 [115 pref/120 metric] updated 01:11:51 ago
         via 20.32.175.175, Ethernet5
>I    20.157.195.0/24 [115 pref/130 metric] updated 01:11:51 ago
         via 20.32.175.175, Ethernet5
>I    20.157.217.0/24 [115 pref/130 metric] updated 01:11:51 ago
         via 20.32.175.175, Ethernet5
>I    20.175.179.0/24 [115 pref/110 metric] updated 01:11:51 ago
         via 20.32.175.175, Ethernet5
>I    20.175.184.0/24 [115 pref/110 metric] updated 01:11:51 ago
         via 20.32.175.175, Ethernet5
>I    20.175.214.0/24 [115 pref/85 metric] updated 00:41:29 ago
         via 20.32.175.175, Ethernet5
>I    20.175.216.0/24 [115 pref/110 metric] updated 01:11:51 ago
         via 20.32.175.175, Ethernet5
>I    30.122.190.0/24 [115 pref/110 metric] updated 01:11:51 ago
         via 20.30.32.30, Ethernet1
>I    101.64.122.0/24 [115 pref/110 metric] updated 01:11:51 ago
         via 20.30.32.30, Ethernet1
>I    101.74.122.0/24 [115 pref/110 metric] updated 01:11:51 ago
         via 20.30.32.30, Ethernet1
>I    101.88.122.0/24 [115 pref/110 metric] updated 01:11:51 ago
         via 20.30.32.30, Ethernet1
>I    101.119.122.0/24 [115 pref/110 metric] updated 01:11:51 ago
         via 20.30.32.30, Ethernet1
>I    101.122.125.0/24 [115 pref/110 metric] updated 01:11:51 ago
         via 20.30.32.30, Ethernet1
>I    101.122.130.0/24 [115 pref/110 metric] updated 01:11:51 ago
         via 20.30.32.30, Ethernet1
>I    101.122.158.0/24 [115 pref/110 metric] updated 01:11:51 ago
         via 20.30.32.30, Ethernet1
>I    101.122.162.0/24 [115 pref/110 metric] updated 01:11:51 ago
         via 20.30.32.30, Ethernet1
>I    101.122.169.0/24 [115 pref/110 metric] updated 01:11:51 ago
         via 20.30.32.30, Ethernet1
>I    101.122.216.0/24 [115 pref/110 metric] updated 01:11:51 ago
         via 20.30.32.30, Ethernet1
>I    101.122.218.0/24 [115 pref/110 metric] updated 01:11:51 ago
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
>C    2001:0:30:32::/64 [0 pref/0 metric] updated 18:04:52 ago
         via Ethernet1, directly connected
>C    2001:0:32:175::/64 [0 pref/0 metric] updated 5d19h ago
         via Ethernet5, directly connected
>C    2002::32/128 [0 pref/0 metric] updated 6d20h ago
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
>P    ::/96 [1 pref/0 metric] updated 9d00h ago
         via Null0, directly connected [NF]
>P    ::ffff:127.0.0.0/104 [1 pref/0 metric] updated 9d00h ago
         via :: [1 pref/1 metric] type ipv6
            via , directly connected
>P    fe80::/10 [1 pref/0 metric] updated 9d00h ago
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
>I    2000::214/128 [115 pref/20 metric] updated 17:42:38 ago
         via fe80::3e08:cdff:fe8d:badc, Ethernet5
>I    2001:0:30:31::/64 [115 pref/20 metric] updated 17:44:04 ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
>I    2001:0:30:66::/64 [115 pref/20 metric] updated 17:44:04 ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
>I    2001:0:30:72::/64 [115 pref/20 metric] updated 17:44:04 ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
>I    2001:0:30:84::/64 [115 pref/20 metric] updated 17:44:04 ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
>I    2001:0:30:120::/64 [115 pref/20 metric] updated 17:17:52 ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
>I    2001:0:30:214::/64 [115 pref/20 metric] updated 17:44:04 ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
>I    2001:0:53:175::/64 [115 pref/20 metric] updated 17:42:38 ago
         via fe80::3e08:cdff:fe8d:badc, Ethernet5
>I    2001:0:66:175::/64 [115 pref/20 metric] updated 17:42:49 ago
         via fe80::3e08:cdff:fe8d:badc, Ethernet5
>I    2001:0:72:175::/64 [115 pref/20 metric] updated 17:42:49 ago
         via fe80::3e08:cdff:fe8d:badc, Ethernet5
>I    2001:0:120:175::/64 [115 pref/20 metric] updated 17:42:49 ago
         via fe80::3e08:cdff:fe8d:badc, Ethernet5
>I    2001:0:128:175::/64 [115 pref/20 metric] updated 17:42:49 ago
         via fe80::3e08:cdff:fe8d:badc, Ethernet5
>I    2001:0:175::/64 [115 pref/20 metric] updated 17:42:49 ago
         via fe80::3e08:cdff:fe8d:badc, Ethernet5
>I    2001:0:175:184::/64 [115 pref/20 metric] updated 17:42:49 ago
         via fe80::3e08:cdff:fe8d:badc, Ethernet5
>I    2001:0:175:214::/64 [115 pref/20 metric] updated 17:42:49 ago
         via fe80::3e08:cdff:fe8d:badc, Ethernet5
>I    2001:0:175:217::/64 [115 pref/20 metric] updated 17:42:49 ago
         via fe80::3e08:cdff:fe8d:badc, Ethernet5
>I    2002::30/128 [115 pref/20 metric] updated 17:44:04 ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
>I    2002::31/128 [115 pref/30 metric] updated 17:24:40 ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
>I    2002::53/128 [115 pref/20 metric] updated 17:42:38 ago
         via fe80::3e08:cdff:fe8d:badc, Ethernet5
>I    2002::175/128 [115 pref/10 metric] updated 17:42:49 ago
         via fe80::3e08:cdff:fe8d:badc, Ethernet5
```

## show platform sand l3 summary

```text
Number of vrfs: 4

Ipv4:
  Routes:       81  backlog:  0  unprogrammed:  0
  Adjacencies:  61  backlog:  0  unprogrammed:  0
Ipv6:
  Routes:       33  backlog:  0  unprogrammed:  0
  Adjacencies:  61  backlog:  0  unprogrammed:  0
Mpls:
  Routes:       34  backlog:  0  unprogrammed:  0
  Adjacencies:  10  backlog:  0  unprogrammed:  0

Jericho2 Ip Fecs:
  Non-ecmp fecs:  4116  ecmp fecs:  0  fec entries:  4116
Jericho2 Mpls Fecs:
  Non-ecmp fecs:  10  ecmp fecs:  0  fec entries:  10
Jericho2 Vxlan Tunnel Fecs:
  Non-ecmp fecs:  0  ecmp fecs:  0  fec entries:  0
  Number of vxlan tunnels configured: 0

Jericho2 Lpm Routes:
  Routes:   81  unprogrammed:   0   
  Routes6:  33  unprogrammed6:  0   
  Backlog:  0 

Jericho2 Lpm:
  TCAM entries used:   4   Percent free:  99  ADS2 entries used:   6  Percent free:  99
  Pivot buckets used:  6   Rows used:     2   Entries Per Bucket:  1  Percent free:  99
  Route buckets used:  24  Rows used:     3   Entries Per Bucket:  4  Percent free:  99

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
  FixedSystem: 6
Egress Mpls (for inner 2 labels) rewrite entries in use (in each fap):
  FixedSystem: 2
Egress Sflow rewrite entries in use (in each fap):
  FixedSystem: 0

Egress rewrite chains in backlog: resource-full 0, no-interface 0

Glem entries used per fap :
  FixedSystem: 4106

Jericho2 Fec:
  Maximum FEC hierarchy levels:  2
  ReusedEcmp:  5  allocs:  5991  frees:  5964  shuffles:  0  cmds:  0
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
    Non-ecmp fecs:            16  ecmp fecs:            0  
    Non-ecmp (Percent free):  99  ecmp (Percent free):  100
  Level3  Fecs:
    Non-ecmp fecs:            38  ecmp fecs:            0  
    Non-ecmp (Percent free):  99  ecmp (Percent free):  100

Lpm Detail:
  Requests:  13425  cleanses:  2237  batches:  2237  avg batch size:  6

Jericho Arp:
  ArpTable writes:      141714  queued      0   
  IngressTable writes:  161699  queued      0   
  Coprocessors:         1       in CmdRing

Tunnel Counter Status
  Number of MPLS tunnels:                  8    
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
|0  |0.0.0.0/8         |DROP | DROP               |0    |  -     |                   |  -  |528526|   -   
|0  |10.0.0.30/32      |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |528528|   -   
|0  |10.0.0.31/32      |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |528528|   -   
|0  |10.0.0.32/32      |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |524291|   -   
|0  |10.0.0.53/32      |ROUTE| Et5                |1010 |107519  | 3c:08:cd:8d:ba:dc |  -  |528486|   -   
|0  |10.0.0.66/32      |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |528528|   -   
|0  |10.0.0.72/32      |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |528528|   -   
|0  |10.0.0.84/32      |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |528528|   -   
|0  |10.0.0.120/32     |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |528528|   -   
|0  |10.0.0.122/32     |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |528528|   -   
|0  |10.0.0.128/32     |ROUTE| Et5                |1010 |107519  | 3c:08:cd:8d:ba:dc |  -  |528486|   -   
|0  |10.0.0.157/32     |ROUTE| Et5                |1010 |107519  | 3c:08:cd:8d:ba:dc |  -  |528486|   -   
|0  |10.0.0.175/32     |ROUTE| Et5                |1010 |107519  | 3c:08:cd:8d:ba:dc |  -  |528486|   -   
|0  |10.0.0.179/32     |ROUTE| Et5                |1010 |107519  | 3c:08:cd:8d:ba:dc |  -  |528486|   -   
|0  |10.0.0.184/32     |ROUTE| Et5                |1010 |107519  | 3c:08:cd:8d:ba:dc |  -  |528486|   -   
|0  |10.0.0.195/32     |ROUTE| Et5                |1010 |107519  | 3c:08:cd:8d:ba:dc |  -  |528486|   -   
|0  |10.0.0.214/32     |ROUTE| Et5                |1010 |107519  | 3c:08:cd:8d:ba:dc |  -  |528486|   -   
|0  |10.0.0.216/32     |ROUTE| Et5                |1010 |107519  | 3c:08:cd:8d:ba:dc |  -  |528486|   -   
|0  |10.0.0.217/32     |ROUTE| Et5                |1010 |107519  | 3c:08:cd:8d:ba:dc |  -  |528486|   -   
|0  |20.30.31.0/24     |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |528528|   -   
|0  |20.30.32.0/32     |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |524290|   -   
|0  |20.30.32.30/32    |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |528484|   -   
|0  |20.30.32.32/32    |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |524291|   -   
|0  |20.30.32.255/32   |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |524290|   -   
|0  |20.30.32.0/24     |TRAP | CoppSystemL3DstMiss|1006 |1006    | ArpTrap           |  -  |525301|   -   
|0  |20.30.66.0/24     |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |528528|   -   
|0  |20.30.72.0/24     |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |528528|   -   
|0  |20.30.84.0/24     |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |528528|   -   
|0  |20.30.120.0/24    |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |528528|   -   
|0  |20.30.122.0/24    |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |528528|   -   
|0  |20.30.214.0/24    |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |528528|   -   
|0  |20.32.175.0/32    |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |524290|   -   
|0  |20.32.175.32/32   |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |524291|   -   
|0  |20.32.175.175/32  |ROUTE| Et5                |1010 |107519  | 3c:08:cd:8d:ba:dc |  -  |528596|   -   
|0  |20.32.175.255/32  |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |524290|   -   
|0  |20.32.175.0/24    |TRAP | CoppSystemL3DstMiss|1010 |1010    | ArpTrap           |  -  |525305|   -   
|0  |20.53.66.0/24     |ROUTE| Et5                |1010 |107519  | 3c:08:cd:8d:ba:dc |  -  |528486|   -   
|0  |20.53.72.0/24     |ROUTE| Et5                |1010 |107519  | 3c:08:cd:8d:ba:dc |  -  |528486|   -   
|0  |20.53.120.0/24    |ROUTE| Et5                |1010 |107519  | 3c:08:cd:8d:ba:dc |  -  |528486|   -   
|0  |20.53.175.0/24    |ROUTE| Et5                |1010 |107519  | 3c:08:cd:8d:ba:dc |  -  |528486|   -   
|0  |20.66.175.0/24    |ROUTE| Et5                |1010 |107519  | 3c:08:cd:8d:ba:dc |  -  |528486|   -   
|0  |20.72.175.0/24    |ROUTE| Et5                |1010 |107519  | 3c:08:cd:8d:ba:dc |  -  |528486|   -   
|0  |20.120.175.0/24   |ROUTE| Et5                |1010 |107519  | 3c:08:cd:8d:ba:dc |  -  |528486|   -   
|0  |20.128.157.0/24   |ROUTE| Et5                |1010 |107519  | 3c:08:cd:8d:ba:dc |  -  |528486|   -   
|0  |20.128.175.0/24   |ROUTE| Et5                |1010 |107519  | 3c:08:cd:8d:ba:dc |  -  |528486|   -   
|0  |20.128.217.0/24   |ROUTE| Et5                |1010 |107519  | 3c:08:cd:8d:ba:dc |  -  |528486|   -   
|0  |20.157.195.0/24   |ROUTE| Et5                |1010 |107519  | 3c:08:cd:8d:ba:dc |  -  |528486|   -   
|0  |20.157.217.0/24   |ROUTE| Et5                |1010 |107519  | 3c:08:cd:8d:ba:dc |  -  |528486|   -   
|0  |20.175.179.0/24   |ROUTE| Et5                |1010 |107519  | 3c:08:cd:8d:ba:dc |  -  |528486|   -   
|0  |20.175.184.0/24   |ROUTE| Et5                |1010 |107519  | 3c:08:cd:8d:ba:dc |  -  |528486|   -   
|0  |20.175.214.0/24   |ROUTE| Et5                |1010 |107519  | 3c:08:cd:8d:ba:dc |  -  |528486|   -   
|0  |20.175.216.0/24   |ROUTE| Et5                |1010 |107519  | 3c:08:cd:8d:ba:dc |  -  |528486|   -   
|0  |30.122.190.0/24   |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |528528|   -   
|0  |101.64.122.0/24   |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |528528|   -   
|0  |101.74.122.0/24   |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |528528|   -   
|0  |101.88.122.0/24   |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |528528|   -   
|0  |101.119.122.0/24  |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |528528|   -   
|0  |101.122.125.0/24  |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |528528|   -   
|0  |101.122.130.0/24  |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |528528|   -   
|0  |101.122.158.0/24  |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |528528|   -   
|0  |101.122.162.0/24  |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |528528|   -   
|0  |101.122.169.0/24  |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |528528|   -   
|0  |101.122.216.0/24  |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |528528|   -   
|0  |101.122.218.0/24  |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |528528|   -   
|0  |127.0.0.0/8       |TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |  -  |524295|   -   
|0  |209.209.209.201/32|TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |524291|   -   
|0  |209.209.209.202/32|TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |524291|   -   
|0  |0.0.0.0/0         |TRAP | CoppSystemL3LpmOver|0    |  -     | SlowReceive       |  -  |524293|   -   
|1  |0.0.0.0/8         |DROP | DROP               |0    |  -     |                   |  -  |528542|   -   
|1  |127.0.0.0/8       |TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |  -  |524295|   -   
|1  |192.168.20.0/32   |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |524290|   -   
|1  |192.168.20.32/32  |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |524291|   -   
|1  |192.168.21.255/32 |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |524290|   -   
|1  |192.168.20.0/23   |TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |  -  |524295|   -   
|1  |0.0.0.0/0         |TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |  -  |524295|   -   
|2  |0.0.0.0/8         |DROP | DROP               |0    |  -     |                   |  -  |528538|   -   
|2  |127.0.0.0/8       |TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |  -  |524295|   -   
|2  |0.0.0.0/0         |TRAP | CoppSystemL3LpmOver|0    |  -     | SlowReceive       |  -  |524293|   -   
|3  |0.0.0.0/8         |DROP | DROP               |0    |  -     |                   |  -  |528544|   -   
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
|  -  |288360|ROUTE| FEC 528494         |   - |2097151 |                 - |Mswap 20179 0
|  -  |288362|ROUTE| FEC 528496         |   - |2097150 |                 - |Mpush 20031
|  -  |288364|ROUTE| FEC 528496         |   - |2097149 |                 - |Mswap 20084 20084
|  -  |288366|ROUTE| FEC 528494         |   - |2097145 |                 - |Mswap 20053 10053
|  -  |288368|ROUTE| FEC 528494         |   - |2097144 |                 - |Mswap 20184 20184
|  -  |288370|ROUTE| FEC 528494         |   - |2097147 |                 - |Mswap 20216 20216
|  -  |288372|ROUTE| FEC 528496         |   - |2097148 |                 - |Mpush 20072
|  -  |288374|ROUTE| FEC 528494         |   - |2097146 |                 - |Mswap 20128 20128
|  -  |524290|TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |   -   
|  -  |524291|TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |   -   
|  -  |524293|TRAP | CoppSystemL3LpmOver|0    |  -     | SlowReceive       |   -   
|  -  |524295|TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |   -   
|  -  |525301|TRAP | CoppSystemL3DstMiss|1006 |1006    | ArpTrap           |   -   
|  -  |525305|TRAP | CoppSystemL3DstMiss|1010 |1010    | ArpTrap           |   -   
|  -  |528482|DROP | DROP               |0    |  -     |                   |   -   
|  -  |528484|ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |   -   
|  -  |528486|ROUTE| Et5                |1010 |107519  | 3c:08:cd:8d:ba:dc |   -   
|  -  |528488|ROUTE| Et5                |1010 |107519  | 3c:08:cd:8d:ba:dc |   -   
|  -  |528490|ROUTE| Et5                |1010 |107519  | 3c:08:cd:8d:ba:dc |   -   
|  -  |528492|ROUTE| Et5                |1010 |107519  | 3c:08:cd:8d:ba:dc |   -   
|  -  |528494|ROUTE| Et5                |1010 |107519  | 3c:08:cd:8d:ba:dc |   -   
|  -  |528496|ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |   -   
|  -  |528526|DROP | DROP               |0    |  -     |                   |   -   
|  -  |528528|ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |   -   
|  -  |528530|ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |   -   
|  -  |528532|ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |   -   
|  -  |528534|ROUTE| Et5                |1010 |107519  | 3c:08:cd:8d:ba:dc |   -   
|  -  |528536|DROP | DROP               |0    |  -     |                   |   -   
|  -  |528538|DROP | DROP               |0    |  -     |                   |   -   
|  -  |528540|ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |   -   
|  -  |528542|DROP | DROP               |0    |  -     |                   |   -   
|  -  |528544|DROP | DROP               |0    |  -     |                   |   -   
|  -  |528596|ROUTE| Et5                |1010 |107519  | 3c:08:cd:8d:ba:dc |   -   

```

## show interfaces counters queue | nz

```text
Aggregate VoQ Counters
Egress                     Traffic               Pkts             Octets           DropPkts         DropOctets
Port                       Class  
--------------------------------------------------------------------------------------------------------------
Et1                        TC1                1233233          123217950                  0                  0
Et1                        TC6                   4869             388783                  0                  0
Et1                        TC7                 267784           74145548                  0                  0
Et2                        TC1                    155              17428                  0                  0
Et2                        TC7                  27834           13139522                  0                  0
Et5                        TC1                1097670          109828066                  0                  0
Et5                        TC6                  20074            1728379                  0                  0
Et5                        TC7                 343908           90534647                  0                  0
Et7                        TC7                   3081             422048                  0                  0
Et40                       TC1               37076394         3559333152                  0                  0
Et40                       TC7                  16707            3698971                  0                  0

Egress Queue Counters
Port                 Traffic DropPrec   DestType          OutEnqPkts      OutEnqOctets       OutDropPkts     OutDropOctets
                     Class
Et1                  TC1     DP0-3      UC                   1233241         123218638                 0                 0
Et1                  TC6     DP0-3      UC                      4869            388763                 0                 0
Et1                  TC7     DP0-3      UC                    267784          73010981                 0                 0
Et2                  TC1     DP0-3      UC                       155             17428                 0                 0
Et2                  TC7     DP0-3      UC                     27834          13044329                 0                 0
Et5                  TC1     DP0-3      UC                   1097662         109827234                 0                 0
Et5                  TC6     DP0-3      UC                     20074           1728379                 0                 0
Et5                  TC7     DP0-3      UC                    343908          88984406                 0                 0
Et7                  TC7     DP0-3      UC                      3081            400481                 0                 0
Et40                 TC1     DP0-3      UC                  37076394        3559333152                 0                 0
Et40                 TC7     DP0-3      UC                     16707           3582022                 0                 0

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
Et1                        TC1                1233233          123217950                  0                  0
Et1                        TC6                   4869             388783                  0                  0
Et1                        TC7                 267784           74145548                  0                  0
Et2                        TC1                    155              17428                  0                  0
Et2                        TC7                  27834           13139522                  0                  0
Et5                        TC1                1097670          109828066                  0                  0
Et5                        TC6                  20074            1728379                  0                  0
Et5                        TC7                 343908           90534647                  0                  0
Et7                        TC7                   3081             422048                  0                  0
Et40                       TC1               37076394         3559333152                  0                  0
Et40                       TC7                  16707            3698971                  0                  0

Egress Queue Counters
Port                 Traffic DropPrec   DestType          OutEnqPkts      OutEnqOctets       OutDropPkts     OutDropOctets
                     Class
Et1                  TC1     DP0-3      UC                   1233241         123218638                 0                 0
Et1                  TC6     DP0-3      UC                      4869            388763                 0                 0
Et1                  TC7     DP0-3      UC                    267784          73010981                 0                 0
Et2                  TC1     DP0-3      UC                       155             17428                 0                 0
Et2                  TC7     DP0-3      UC                     27834          13044329                 0                 0
Et5                  TC1     DP0-3      UC                   1097662         109827234                 0                 0
Et5                  TC6     DP0-3      UC                     20074           1728379                 0                 0
Et5                  TC7     DP0-3      UC                    343908          88984406                 0                 0
Et7                  TC7     DP0-3      UC                      3081            400481                 0                 0
Et40                 TC1     DP0-3      UC                  37076394        3559333152                 0                 0
Et40                 TC7     DP0-3      UC                     16707           3582022                 0                 0

```

