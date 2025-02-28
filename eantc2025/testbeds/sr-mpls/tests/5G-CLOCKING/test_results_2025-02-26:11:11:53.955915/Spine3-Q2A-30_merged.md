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

Uptime: 5 days, 20 hours and 34 minutes
Total memory: 8099700 kB
Free memory: 4781492 kB

```

## show interfaces counters rates | nz

```text
Port      Name                 Intvl  In Mbps      %  In Kpps Out Mbps      %
Et9       Ciena-5134-72 port 2  0:01      0.0   0.0%        0      0.0   0.0%
Et11      Juniper-156 port 590  0:01      0.0   0.0%        0      0.0   0.0%
Et21      Juniper-156 port 592  0:01      0.0   0.0%        0      0.0   0.0%
Et31      Ciena-8140-66 port 2  0:01   8000.0  96.7%    10416   8333.3 100.0%
Et35      Juniper-131-JCNR 42   0:01      0.0   0.0%        0      0.0   0.0%
Et46/1    Arista-Harness3       0:01   9607.5  11.6%    12509   7999.9   9.7%

Port      Out Kpps
Et31         10416
Et46/1       10416
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
Ethernet7          20.30.184.30/24    down         down           1500         
Ethernet8          21.30.217.30/24    admin down   down           1500         
Ethernet9          20.30.72.30/24     admin down   down           1500         
Ethernet10         21.30.120.30/24    admin down   down           1500         
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
2-23-5G   default  Ciena-8140-66    L2   Ethernet31         P2P               UP    27          02                  
```

## show isis database detail

```text
Legend:
H - hostname conflict
U - node unreachable

IS-IS Instance: 2-23-5G VRF: default
  IS-IS Level 2 Link State Database
    LSPID                   Seq Num  Cksum  Life Length IS  Received LSPID        Flags
    Arrcus-53.00-00            1667  64048   714    441 L2  0000.0000.0053.00-00  <>
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
      IS Neighbor          : 0000.0000.0128.00   Metric: 10
        IPv4 Neighbor Address: 20.53.128.128
        IPv4 Interface Address: 20.53.128.53
      IS Neighbor          : Nokia-IXRe2-216.00  Metric: 10
        IPv4 Neighbor Address: 20.53.216.216
        IPv4 Interface Address: 20.53.216.53
      IS Neighbor (MT-IPv6): Nokia-IXRe2-216.00  Metric: 10
        IPv4 Interface Address: 20.53.216.53
      Reachability         : 20.53.66.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.53.72.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.53.120.0/24 Metric: 10 Type: 1 Up
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
        Algorithms:  0
    Arrcus-72XC-2-54.00-00       320  34287   975    165 L2  0000.0000.0054.00-00  <>
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
    Ciena-8140-66.00-00         426  55868   780    809 L2  0000.0000.0066.00-00  <>
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
      IS Neighbor          : Juniper-156-PTX10002-36QDD.00 Metric: 10
        IPv4 Neighbor Address: 20.66.156.156
        IPv4 Interface Address: 20.66.156.66
        Adj-sid: 16019 flags: [L V] weight: 0x0
      IS Neighbor          : Nokia-SXR-214.00    Metric: 10
        IPv4 Neighbor Address: 20.66.214.214
        IPv4 Interface Address: 20.66.214.66
        Adj-sid: 16015 flags: [L V] weight: 0x0
      IS Neighbor          : Arrcus-72XC-2-54.00 Metric: 10
        IPv4 Neighbor Address: 20.54.66.54
        IPv4 Interface Address: 20.54.66.66
        Adj-sid: 16018 flags: [L V] weight: 0x0
      IS Neighbor          : Arrcus-53.00        Metric: 10
        IPv4 Neighbor Address: 20.53.66.53
        IPv4 Interface Address: 20.53.66.66
        Adj-sid: 16016 flags: [L V] weight: 0x0
      Reachability         : 10.0.0.66/32 Metric: 10 Type: 1 Up
        SR Prefix-SID: 66 Flags: [N] Algorithm: 0
      Reachability         : 20.30.66.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.66.84.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.54.66.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.66.179.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.66.156.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.66.214.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.53.66.0/24 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.66 Flags: []
        SR Capability: Flags: [I]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0
    Ciena-5134-72.00-00         203  52227   305    209 L2  0000.0000.0072.00-00  <>
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
    Ericsson_84_R6678.00-00       195  46023   683    187 L2  0000.0000.0084.00-00  <>
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
    H3C_M1A_120.00-00         24956  42406  1194    547 L2  0000.0000.0120.00-00  <>
      Remaining lifetime received: 13 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: H3C_M1A_120
      Area addresses: 49.0001
      Topology: 0 (IPv4)
      Topology: 2 (IPv6)
      Interface address: 10.0.0.120
      Interface address: 20.53.120.120
      Interface address: 2002::120
      IS Neighbor          : Arrcus-53.00        Metric: 2
        IPv4 Neighbor Address: 20.53.120.53
        IPv4 Interface Address: 20.53.120.120
        Adj-sid: 1151 flags: [L V] weight: 0x0
      IS Neighbor          : Arrcus-53.00        Metric: 2
        IPv4 Neighbor Address: 20.53.120.53
        IPv4 Interface Address: 20.53.120.120
      Reachability         : 10.0.0.120/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 120 Flags: [N] Algorithm: 0
        SR Prefix-SID: 1248 Flags: [N] Algorithm: 128
        SR Prefix-SID: 1249 Flags: [N] Algorithm: 129
        SR Prefix-SID: 1250 Flags: [N] Algorithm: 130
      Reachability         : 20.53.120.0/24 Metric: 2 Type: 1 Up
      Reachability         : 20.120.217.0/24 Metric: 0 Type: 1 Up
      Reachability         : 50.20.120.0/24 Metric: 0 Type: 1 Up
      Reachability         : 192.168.20.0/23 Metric: 0 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:53:120::/64 Metric: 0 Type: 1 Up
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
    0000.0000.0128.00-00       2193  26302  1123    268 L2  0000.0000.0128.00-00  <>
      Remaining lifetime received: 1198 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Area addresses: 49.0001
      Topology: 0 (IPv4)
      Topology: 2 (IPv6)
      Interface address: 10.0.0.128
      Interface address: 20.53.128.128
      Interface address: 20.128.157.128
      Interface address: 20.128.217.128
      IS Neighbor          : Arrcus-53.00        Metric: 10
        IPv4 Neighbor Address: 20.53.128.53
        IPv4 Interface Address: 20.53.128.128
        Adj-sid: 48000 flags: [L V] weight: 0x0
      IS Neighbor          : Juniper-157-PTX10002-36QDD.00 Metric: 10
        IPv4 Neighbor Address: 20.128.157.157
        IPv4 Interface Address: 20.128.157.128
        Adj-sid: 48001 flags: [L V] weight: 0x0
      IS Neighbor          : Nokia-SR1-217.00    Metric: 10
        IPv4 Neighbor Address: 20.128.217.217
        IPv4 Interface Address: 20.128.217.128
        Adj-sid: 48002 flags: [L V] weight: 0x0
      Reachability         : 10.0.0.128/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 128 Flags: [N] Algorithm: 0
      Reachability         : 20.53.128.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.128.157.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.128.217.0/24 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.128 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  10
        SR Capability: Flags: [I]
          SRGB Base: 20000 Range: 2000
    Keys195.00-00                 9  46026  1177    158 L2  0000.0000.0195.00-00  <DefaultAtt>
      Remaining lifetime received: 1199 s Modified to: 1200 s
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
    Nokia-SXR-214.00-00       32634  56740  1128    257 L2  0000.0000.0214.00-00  <>
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
        Adj-sid: 30046 flags: [L V B] weight: 0x0
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
    Arista-Spine3-Q2A-2-23.00-00       210  30764   445    167 L2  0000.0000.3030.00-00  <>
      LSP generation remaining wait time: 0 ms
      Time remaining until refresh: 145 s
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
    Juniper-156-PTX10002-36QDD.00-00       231  22384   491    291 L2  0000.0001.0156.00-00  <>
      Remaining lifetime received: 1198 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Juniper-156-PTX10002-36QDD
      Area addresses: 49.0001
      Interface address: 10.0.0.156
      Interface address: 10.0.1.156
      Interface address: 2002::156
      IS Neighbor          : Ciena-8140-66.00    Metric: 10
        IPv4 Neighbor Address: 20.66.156.66
        IPv4 Interface Address: 20.66.156.156
        Adj-sid: 35 flags: [L V] weight: 0x0
      IS Neighbor          : Nokia-IXRe2-216.00  Metric: 10
        IPv4 Neighbor Address: 20.156.216.216
        IPv4 Interface Address: 20.156.216.156
        Adj-sid: 28 flags: [L V] weight: 0x0
      Reachability         : 10.0.1.156/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 456 Flags: [N] Algorithm: 0
      Router Capabilities: Router Id: 10.0.0.156 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  0
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0, 1
      Unsupported TLV: Type: 14 Length: 2
    Juniper-179-ACX7024.00-00       688  28816   850    222 L2  0000.0001.0179.00-00  <>
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
    Nokia-IXRe2-216.00-00      2009  26490  1023    322 L2  0100.0000.0216.00-00  <>
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
    Nokia-SR1-217.00-00         286  51819   801    225 L2  0100.0000.0217.00-00  <>
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
        Adj-sid: 524270 flags: [L V B] weight: 0x0
      IS Neighbor          : 0000.0000.0128.00   Metric: 10
        IPv4 Neighbor Address: 20.128.217.128
        IPv4 Interface Address: 20.128.217.217
        Adj-sid: 524267 flags: [L V B] weight: 0x0
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
    Juniper-157-PTX10002-36QDD.00-00       236  13245   609    304 L2  1000.0000.0157.00-00  <>
      Remaining lifetime received: 1198 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Juniper-157-PTX10002-36QDD
      Area addresses: 49.0001.0000.0000
      Interface address: 10.0.0.157
      IS Neighbor          : 0000.0000.0128.00   Metric: 10
        IPv4 Neighbor Address: 20.128.157.128
        IPv4 Interface Address: 20.128.157.157
        Adj-sid: 22 flags: [L V] weight: 0x0
      IS Neighbor          : Nokia-SR1-217.00    Metric: 10
        IPv4 Neighbor Address: 20.157.217.217
        IPv4 Interface Address: 20.157.217.157
        Adj-sid: 21 flags: [L V] weight: 0x0
      IS Neighbor          : Keys195.00          Metric: 10
        IPv4 Neighbor Address: 20.157.195.195
        IPv4 Interface Address: 20.157.195.157
        Adj-sid: 24 flags: [L V] weight: 0x0
      Reachability         : 10.0.0.157/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 157 Flags: [N] Algorithm: 0
      Reachability         : 20.157.217.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.128.157.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.157.195.0/24 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.157 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  0
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0, 1
      Unsupported TLV: Type: 14 Length: 2

Legend:
H - hostname conflict
U - node unreachable

IS-IS Instance: IGP VRF: default
  IS-IS Level 2 Link State Database
    LSPID                   Seq Num  Cksum  Life Length IS  Received LSPID        Flags
    Arista-Spine3-Q2A-30.00-00      7115  65350   423    265 L2  0000.0000.0030.00-00  <>
      LSP generation remaining wait time: 0 ms
      Time remaining until refresh: 123 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Arista-Spine3-Q2A-30
      Area addresses: 49.0001
      Topology: 2 (IPv6)
      Topology: 0 (IPv4)
      Interface address: 10.0.0.30
      Interface address: 2002::30
      Reachability         : 10.0.0.30/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 30 Flags: [N] Algorithm: 0
        SR Prefix-SID: 158 Flags: [N] Algorithm: 128
        SR Prefix-SID: 159 Flags: [N] Algorithm: 129
        SR Prefix-SID: 160 Flags: [N] Algorithm: 130
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

```

## show isis database traffic-engineering

```text
Legend:
H - hostname conflict
U - node unreachable

IS-IS Instance: 2-23-5G VRF: default
  IS-IS Level 2 Link State Database
    LSPID                   Seq Num  Cksum  Life Length IS  Received LSPID        Flags
    Arrcus-53.00-00            1667  64048   714    441 L2  0000.0000.0053.00-00  <>
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
      IS Neighbor          : 0000.0000.0128.00   Metric: 10
        IPv4 Neighbor Address: 20.53.128.128
        IPv4 Interface Address: 20.53.128.53
      IS Neighbor          : Nokia-IXRe2-216.00  Metric: 10
        IPv4 Neighbor Address: 20.53.216.216
        IPv4 Interface Address: 20.53.216.53
      IS Neighbor (MT-IPv6): Nokia-IXRe2-216.00  Metric: 10
        IPv4 Interface Address: 20.53.216.53
      Reachability         : 20.53.66.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.53.72.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.53.120.0/24 Metric: 10 Type: 1 Up
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
        Algorithms:  0
    Arrcus-72XC-2-54.00-00       320  34287   975    165 L2  0000.0000.0054.00-00  <>
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
    Ciena-8140-66.00-00         426  55868   780    809 L2  0000.0000.0066.00-00  <>
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
        Remote link ID: 1044
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
      Reachability         : 10.0.0.66/32 Metric: 10 Type: 1 Up
        SR Prefix-SID: 66 Flags: [N] Algorithm: 0
      Reachability         : 20.30.66.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.66.84.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.54.66.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.66.179.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.66.156.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.66.214.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.53.66.0/24 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.66 Flags: []
        SR Capability: Flags: [I]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0
    Ciena-5134-72.00-00         203  52227   305    209 L2  0000.0000.0072.00-00  <>
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
    Ericsson_84_R6678.00-00       195  46023   683    187 L2  0000.0000.0084.00-00  <>
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
    H3C_M1A_120.00-00         24956  42406  1194    547 L2  0000.0000.0120.00-00  <>
      Remaining lifetime received: 13 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: H3C_M1A_120
      TE IPv4 router ID: 10.0.0.120
      Area addresses: 49.0001
      Topology: 0 (IPv4)
      Topology: 2 (IPv6)
      Interface address: 10.0.0.120
      Interface address: 20.53.120.120
      Interface address: 2002::120
      IS Neighbor          : Arrcus-53.00        Metric: 2
        IPv4 Neighbor Address: 20.53.120.53
        IPv4 Interface Address: 20.53.120.120
        Adj-sid: 1151 flags: [L V] weight: 0x0
        TE default metric: 2
        Maximum link BW: 0.00 bps
        Maximum reservable link BW: 0.00 bps
        Unreserved BW:
            TE class 0: 0.00 bps	TE class 1: 0.00 bps	TE class 2: 0.00 bps
            TE class 3: 0.00 bps	TE class 4: 0.00 bps	TE class 5: 0.00 bps
            TE class 6: 0.00 bps	TE class 7: 0.00 bps
        Local link ID: 6
        Remote link ID: 1009
      IS Neighbor          : Arrcus-53.00        Metric: 2
        IPv4 Neighbor Address: 20.53.120.53
        IPv4 Interface Address: 20.53.120.120
        Local link ID: 6
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
      Reachability         : 10.0.0.120/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 120 Flags: [N] Algorithm: 0
        SR Prefix-SID: 1248 Flags: [N] Algorithm: 128
        SR Prefix-SID: 1249 Flags: [N] Algorithm: 129
        SR Prefix-SID: 1250 Flags: [N] Algorithm: 130
      Reachability         : 20.53.120.0/24 Metric: 2 Type: 1 Up
      Reachability         : 20.120.217.0/24 Metric: 0 Type: 1 Up
      Reachability         : 50.20.120.0/24 Metric: 0 Type: 1 Up
      Reachability         : 192.168.20.0/23 Metric: 0 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:53:120::/64 Metric: 0 Type: 1 Up
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
    0000.0000.0128.00-00       2193  26302  1123    268 L2  0000.0000.0128.00-00  <>
      Remaining lifetime received: 1198 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      TE IPv4 router ID: 10.0.0.128
      Area addresses: 49.0001
      Topology: 0 (IPv4)
      Topology: 2 (IPv6)
      Interface address: 10.0.0.128
      Interface address: 20.53.128.128
      Interface address: 20.128.157.128
      Interface address: 20.128.217.128
      IS Neighbor          : Arrcus-53.00        Metric: 10
        IPv4 Neighbor Address: 20.53.128.53
        IPv4 Interface Address: 20.53.128.128
        Adj-sid: 48000 flags: [L V] weight: 0x0
        Local link ID: 14
        Remote link ID: 1029
      IS Neighbor          : Juniper-157-PTX10002-36QDD.00 Metric: 10
        IPv4 Neighbor Address: 20.128.157.157
        IPv4 Interface Address: 20.128.157.128
        Adj-sid: 48001 flags: [L V] weight: 0x0
        Local link ID: 13
        Remote link ID: 1048
      IS Neighbor          : Nokia-SR1-217.00    Metric: 10
        IPv4 Neighbor Address: 20.128.217.217
        IPv4 Interface Address: 20.128.217.128
        Adj-sid: 48002 flags: [L V] weight: 0x0
        Local link ID: 8
        Remote link ID: 17
      Reachability         : 10.0.0.128/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 128 Flags: [N] Algorithm: 0
      Reachability         : 20.53.128.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.128.157.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.128.217.0/24 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.128 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  10
        SR Capability: Flags: [I]
          SRGB Base: 20000 Range: 2000
    Keys195.00-00                 9  46026  1177    158 L2  0000.0000.0195.00-00  <DefaultAtt>
      Remaining lifetime received: 1199 s Modified to: 1200 s
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
    Nokia-SXR-214.00-00       32634  56740  1128    257 L2  0000.0000.0214.00-00  <>
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
        Adj-sid: 30046 flags: [L V B] weight: 0x0
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
    Arista-Spine3-Q2A-2-23.00-00       210  30764   445    167 L2  0000.0000.3030.00-00  <>
      LSP generation remaining wait time: 0 ms
      Time remaining until refresh: 145 s
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
    Juniper-156-PTX10002-36QDD.00-00       231  22384   490    291 L2  0000.0001.0156.00-00  <>
      Remaining lifetime received: 1198 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Juniper-156-PTX10002-36QDD
      TE IPv4 router ID: 10.0.0.156
      TE IPv6 router ID: 2002::156
      Area addresses: 49.0001
      Interface address: 10.0.0.156
      Interface address: 10.0.1.156
      Interface address: 2002::156
      IS Neighbor          : Ciena-8140-66.00    Metric: 10
        IPv4 Neighbor Address: 20.66.156.66
        IPv4 Interface Address: 20.66.156.156
        Adj-sid: 35 flags: [L V] weight: 0x0
        Maximum link BW: 100.00 Gbps
        Local link ID: 1044
        Remote link ID: 1073731840
      IS Neighbor          : Nokia-IXRe2-216.00  Metric: 10
        IPv4 Neighbor Address: 20.156.216.216
        IPv4 Interface Address: 20.156.216.156
        Adj-sid: 28 flags: [L V] weight: 0x0
        Maximum link BW: 100.00 Gbps
        Local link ID: 1038
        Remote link ID: 24
      Reachability         : 10.0.1.156/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 456 Flags: [N] Algorithm: 0
      Router Capabilities: Router Id: 10.0.0.156 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  0
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0, 1
      Unsupported TLV: Type: 14 Length: 2
    Juniper-179-ACX7024.00-00       688  28816   850    222 L2  0000.0001.0179.00-00  <>
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
    Nokia-IXRe2-216.00-00      2009  26490  1023    322 L2  0100.0000.0216.00-00  <>
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
    Nokia-SR1-217.00-00         286  51819   801    225 L2  0100.0000.0217.00-00  <>
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
        Adj-sid: 524270 flags: [L V B] weight: 0x0
      IS Neighbor          : 0000.0000.0128.00   Metric: 10
        IPv4 Neighbor Address: 20.128.217.128
        IPv4 Interface Address: 20.128.217.217
        Adj-sid: 524267 flags: [L V B] weight: 0x0
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
    Juniper-157-PTX10002-36QDD.00-00       236  13245   608    304 L2  1000.0000.0157.00-00  <>
      Remaining lifetime received: 1198 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Juniper-157-PTX10002-36QDD
      TE IPv4 router ID: 10.0.0.157
      Area addresses: 49.0001.0000.0000
      Interface address: 10.0.0.157
      IS Neighbor          : 0000.0000.0128.00   Metric: 10
        IPv4 Neighbor Address: 20.128.157.128
        IPv4 Interface Address: 20.128.157.157
        Adj-sid: 22 flags: [L V] weight: 0x0
        Local link ID: 1048
        Remote link ID: 13
      IS Neighbor          : Nokia-SR1-217.00    Metric: 10
        IPv4 Neighbor Address: 20.157.217.217
        IPv4 Interface Address: 20.157.217.157
        Adj-sid: 21 flags: [L V] weight: 0x0
        Local link ID: 1004
        Remote link ID: 10
      IS Neighbor          : Keys195.00          Metric: 10
        IPv4 Neighbor Address: 20.157.195.195
        IPv4 Interface Address: 20.157.195.157
        Adj-sid: 24 flags: [L V] weight: 0x0
        Local link ID: 1040
        Remote link ID: 1
      Reachability         : 10.0.0.157/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 157 Flags: [N] Algorithm: 0
      Reachability         : 20.157.217.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.128.157.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.157.195.0/24 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.157 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  0
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0, 1
      Unsupported TLV: Type: 14 Length: 2

Legend:
H - hostname conflict
U - node unreachable

IS-IS Instance: IGP VRF: default
  IS-IS Level 2 Link State Database
    LSPID                   Seq Num  Cksum  Life Length IS  Received LSPID        Flags
    Arista-Spine3-Q2A-30.00-00      7115  65350   422    265 L2  0000.0000.0030.00-00  <>
      LSP generation remaining wait time: 0 ms
      Time remaining until refresh: 122 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Arista-Spine3-Q2A-30
      TE IPv4 router ID: 10.0.0.30
      Area addresses: 49.0001
      Topology: 2 (IPv6)
      Topology: 0 (IPv4)
      Interface address: 10.0.0.30
      Interface address: 2002::30
      Reachability         : 10.0.0.30/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 30 Flags: [N] Algorithm: 0
        SR Prefix-SID: 158 Flags: [N] Algorithm: 128
        SR Prefix-SID: 159 Flags: [N] Algorithm: 129
        SR Prefix-SID: 160 Flags: [N] Algorithm: 130
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
Last updated: 1 day, 21:43:27 ago
Next Hop Interface
-------- ---------

Destination: Arista-Spine3-Q2A-30
Path ID: 641
Path constraints: algo MIN-TE
                  metric type TE
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 1
Last updated: 1 day, 21:43:27 ago
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
Last updated: 1 day, 21:43:27 ago
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
Last updated: 1 day, 21:43:27 ago
Next Hop Interface
-------- ---------

Destination: Arista-Spine3-Q2A-30
Path ID: 641
Path constraints: algo MIN-TE
                  metric type TE
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 1
Last updated: 1 day, 21:43:27 ago
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
Last updated: 1 day, 21:43:27 ago
Next Hop Interface
-------- ---------

```

## show isis segment-routing tunnel

```text
  Index     Endpoint          Next Hop/Tunnel Index     Interface     Labels   
--------- ----------------- ------------------------- --------------- ---------
  8         10.0.0.84/32      20.30.66.66               Ethernet31    [ 20084 ]
  10        10.0.0.53/32      20.30.66.66               Ethernet31    [ 20053 ]
  13        10.0.0.66/32      20.30.66.66               Ethernet31    [ 3 ]    
  14        10.0.0.72/32      20.30.66.66               Ethernet31    [ 20072 ]
  16        10.0.0.217/32     20.30.66.66               Ethernet31    [ 21217 ]
  17        10.0.0.120/32     20.30.66.66               Ethernet31    [ 20120 ]
  18        10.0.0.128/32     20.30.66.66               Ethernet31    [ 20128 ]
  21        10.0.0.214/32     20.30.66.66               Ethernet31    [ 20214 ]
  23        10.0.1.179/32     20.30.66.66               Ethernet31    [ 20479 ]
  24        10.0.1.156/32     20.30.66.66               Ethernet31    [ 20456 ]
  25        10.0.0.216/32     20.30.66.66               Ethernet31    [ 20216 ]
  29        10.0.0.54/32      20.30.66.66               Ethernet31    [ 20054 ]
  30        10.0.0.157/32     20.30.66.66               Ethernet31    [ 20157 ]
  31        10.0.0.195/32     20.30.66.66               Ethernet31    [ 20195 ]

```

## show isis segment-routing prefix-segments

```text

System ID: Arista-Spine3-Q2A-2-23			Instance: '2-23-5G'
SR supported Data-plane: MPLS			SR Router ID: 10.0.30.30

Node: 21     Proxy-Node: 0      Prefix: 0       Total Segments: 21

Flag Descriptions: R: Re-advertised, N: Node Segment, P: no-PHP
                   E: Explicit-NULL, V: Value, L: Local
Segment status codes: * - Self originated Prefix, L1 - level 1, L2 - level 2, ! - SR-unreachable,
                      # - Some IS-IS next-hops are SR-unreachable
   Prefix                      SID   Label Type       Flags                        System ID       Level Protection  Algorithm   
   ------------------------- ----- ------- ---------- ---------------------------- --------------- ----- ----------- -------------
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
   10.0.0.128/32               128   20128 Node       R:0 N:1 P:0 E:0 V:0 L:0      0000.0000.0128  L2    unprotected SPF         
   10.0.0.157/32               157   20157 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-157-PTX10002-36QDD L2    unprotected SPF         
   10.0.0.195/32               195   20195 Node       R:0 N:1 P:0 E:0 V:0 L:0      Keys195         L2    unprotected SPF         
   10.0.0.214/32               214   20214 Node       R:0 N:1 P:1 E:0 V:0 L:0      Nokia-SXR-214   L2    unprotected SPF         
   10.0.0.216/32               216   20216 Node       R:0 N:1 P:1 E:0 V:0 L:0      Nokia-IXRe2-216 L2    unprotected SPF         
   10.0.0.217/32              1217   21217 Node       R:0 N:1 P:1 E:0 V:0 L:0      Nokia-SR1-217   L2    unprotected SPF         
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
 I L2     10.0.0.128/32 [115/21]
           via 20.30.66.66, Ethernet31
 I L2     10.0.0.157/32 [115/31]
           via 20.30.66.66, Ethernet31
 I L2     10.0.0.195/32 [115/51]
           via 20.30.66.66, Ethernet31
 I L2     10.0.0.214/32 [115/11]
           via 20.30.66.66, Ethernet31
 I L2     10.0.0.216/32 [115/21]
           via 20.30.66.66, Ethernet31
 I L2     10.0.0.217/32 [115/31]
           via 20.30.66.66, Ethernet31
 I L2     10.0.1.156/32 [115/11]
           via 20.30.66.66, Ethernet31
 I L2     10.0.1.179/32 [115/11]
           via 20.30.66.66, Ethernet31
 C        10.0.30.30/32
           directly connected, Loopback1000
 C        20.30.66.0/24
           directly connected, Ethernet31
 I L2     20.53.66.0/24 [115/11]
           via 20.30.66.66, Ethernet31
 I L2     20.53.72.0/24 [115/21]
           via 20.30.66.66, Ethernet31
 I L2     20.53.120.0/24 [115/21]
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
 I L2     20.66.179.0/24 [115/11]
           via 20.30.66.66, Ethernet31
 I L2     20.66.214.0/24 [115/11]
           via 20.30.66.66, Ethernet31
 I L2     20.120.217.0/24 [115/21]
           via 20.30.66.66, Ethernet31
 I L2     20.128.157.0/24 [115/31]
           via 20.30.66.66, Ethernet31
 I L2     20.128.217.0/24 [115/31]
           via 20.30.66.66, Ethernet31
 I L2     20.156.216.0/24 [115/31]
           via 20.30.66.66, Ethernet31
 I L2     20.157.195.0/24 [115/41]
           via 20.30.66.66, Ethernet31
 I L2     20.157.217.0/24 [115/41]
           via 20.30.66.66, Ethernet31
 I L2     50.20.120.0/24 [115/21]
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
           via 10.0.0.120/32, IS-IS SR tunnel index 17, label 1407
              via 20.30.66.66, Ethernet31, label 20120
 B I      50.10.128.0/24 [200/0]
           via 10.0.0.128/32, IS-IS SR tunnel index 18, label 48063
              via 20.30.66.66, Ethernet31, label 20128
 B I      50.10.179.0/24 [200/0]
           via 10.0.1.179/32, IS-IS SR tunnel index 23, label 30
              via 20.30.66.66, Ethernet31, label 20479
 B I      50.10.214.0/24 [200/0]
           via 10.0.0.214/32, IS-IS SR tunnel index 21, label 500001
              via 20.30.66.66, Ethernet31, label 20214
 B I      50.10.216.0/24 [200/0]
           via 10.0.0.216/32, IS-IS SR tunnel index 25, label 1048575
              via 20.30.66.66, Ethernet31, label 20216


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
 B I      50.128.156.0/24 [200/0]
           via 10.0.1.156/32, IS-IS SR tunnel index 24, label 17
              via 20.30.66.66, Ethernet31, label 20456
 B I      50.129.156.0/24 [200/0]
           via 10.0.1.156/32, IS-IS SR tunnel index 24, label 17
              via 20.30.66.66, Ethernet31, label 20456
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
 B I      50.10.156.0/24 [200/0]
           via 10.0.1.156/32, IS-IS SR tunnel index 24, label 16
              via 20.30.66.66, Ethernet31, label 20456
 B I      50.10.179.0/24 [200/0]
           via 10.0.1.179/32, IS-IS SR tunnel index 23, label 16
              via 20.30.66.66, Ethernet31, label 20479
 B I      50.11.156.0/24 [200/0]
           via 10.0.1.156/32, IS-IS SR tunnel index 24, label 16
              via 20.30.66.66, Ethernet31, label 20456


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
Displaying 2 of 6 IPv6 routing table entries
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
 C        2002::30/128 [0/0]
           via Loopback0, directly connected

```

## show mpls route

```text
MPLS forwarding table (Label [metric] Vias) - 19 routes 
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

 20053   A[1]
                via M, forward
                    EgressACL: apply
                    20.30.66.66 Ethernet31
 20054   A[1]
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
 20128   A[1]
                via M, forward
                    EgressACL: apply
                    20.30.66.66 Ethernet31
 20157   A[1]
                via M, forward
                    EgressACL: apply
                    20.30.66.66 Ethernet31
 20195   A[1]
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
 20456   A[1]
                via M, forward
                    EgressACL: apply
                    20.30.66.66 Ethernet31
 20479   A[1]
                via M, forward
                    EgressACL: apply
                    20.30.66.66 Ethernet31
 21217   A[1]
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

 IP    20053    [1], 10.0.0.53/32
                via M, 20.30.66.66, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet31
 IP    20054    [1], 10.0.0.54/32
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
 IP    20128    [1], 10.0.0.128/32
                via M, 20.30.66.66, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet31
 IP    20157    [1], 10.0.0.157/32
                via M, 20.30.66.66, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet31
 IP    20195    [1], 10.0.0.195/32
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
 IP    20456    [1], 10.0.1.156/32
                via M, 20.30.66.66, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet31
 IP    20479    [1], 10.0.1.179/32
                via M, 20.30.66.66, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet31
 IP    21217    [1], 10.0.0.217/32
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
 * >Ec    RD: 6128:128 auto-discovery 128 0000:0000:0000:0000:0000
                                 10.0.0.128            -       100     0       i Or-ID: 10.0.0.128 C-LST: 10.0.0.216 
 *  ec    RD: 6128:128 auto-discovery 128 0000:0000:0000:0000:0000
                                 10.0.0.128            -       100     0       i Or-ID: 10.0.0.128 C-LST: 10.0.1.156 
 * >Ec    RD: 10.0.0.179:65530 auto-discovery 179 0000:0000:0000:0000:0000
                                 10.0.1.179            -       100     0       i Or-ID: 10.0.0.179 C-LST: 10.0.0.216 
 *  ec    RD: 10.0.0.179:65530 auto-discovery 179 0000:0000:0000:0000:0000
                                 10.0.1.179            -       100     0       i Or-ID: 10.0.0.179 C-LST: 10.0.1.156 
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
 * >Ec    RD: 214:128 auto-discovery 214 0000:0000:0000:0000:0000
                                 10.0.0.214            -       100     0       i Or-ID: 10.0.0.214 C-LST: 10.0.0.216 
 *  ec    RD: 214:128 auto-discovery 214 0000:0000:0000:0000:0000
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
          RD: 10.0.0.64:1 auto-discovery 1112 0000:0000:0000:0000:0000
                                 2002::64              -       100     0       65000 i Or-ID: 10.0.0.64 C-LST: 10.0.0.216 100.0.0.155 
          RD: 10.0.0.74:1 auto-discovery 1112 0000:0000:0000:0000:0000
                                 2002::74              -       100     0       65000 i Or-ID: 10.0.0.74 C-LST: 10.0.0.216 100.0.0.155 
          RD: 1113:88 auto-discovery 1113 0000:0000:0000:0000:0000
                                 2002::88              0       100     0       65000 ? Or-ID: 100.0.0.88 C-LST: 10.0.0.216 100.0.0.155 
          RD: 10.0.0.64:2 auto-discovery 1113 0000:0000:0000:0000:0000
                                 2002::64              -       100     0       65000 i Or-ID: 10.0.0.64 C-LST: 10.0.0.216 100.0.0.155 
          RD: 1114:119 auto-discovery 1114 0000:0000:0000:0000:0000
                                 1001::119             0       100     0       65000 i Or-ID: 100.0.0.119 C-LST: 10.0.0.216 100.0.0.155 
          RD: 10.0.0.64:3 auto-discovery 1114 0000:0000:0000:0000:0000
                                 2002::64              -       100     0       65000 i Or-ID: 10.0.0.64 C-LST: 10.0.0.216 100.0.0.155 
          RD: 1115:122 auto-discovery 1115 0000:0000:0000:0000:0000
                                 2002::122             0       100     0       65000 i Or-ID: 100.0.0.122 C-LST: 10.0.0.216 100.0.0.155 
          RD: 10.0.0.64:4 auto-discovery 1115 0000:0000:0000:0000:0000
                                 2002::64              -       100     0       65000 i Or-ID: 10.0.0.64 C-LST: 10.0.0.216 100.0.0.155 
          RD: 1116:125 auto-discovery 1116 0000:0000:0000:0000:0000
                                 2002::125             -       100     0       65000 i Or-ID: 100.0.0.125 C-LST: 10.0.0.216 100.0.0.155 
          RD: 10.0.0.64:5 auto-discovery 1116 0000:0000:0000:0000:0000
                                 2002::64              -       100     0       65000 i Or-ID: 10.0.0.64 C-LST: 10.0.0.216 100.0.0.155 
          RD: 1117:130 auto-discovery 1117 0000:0000:0000:0000:0000
                                 2002::130             -       100     0       65000 i Or-ID: 100.0.0.130 C-LST: 10.0.0.216 100.0.0.155 
          RD: 10.0.0.64:6 auto-discovery 1117 0000:0000:0000:0000:0000
                                 2002::64              -       100     0       65000 i Or-ID: 10.0.0.64 C-LST: 10.0.0.216 100.0.0.155 
          RD: 10.0.0.64:7 auto-discovery 1118 0000:0000:0000:0000:0000
                                 2002::64              -       100     0       65000 i Or-ID: 10.0.0.64 C-LST: 10.0.0.216 100.0.0.155 
          RD: 100.0.0.158:1118 auto-discovery 1118 0000:0000:0000:0000:0000
                                 1001::158             -       100     0       65000 i Or-ID: 100.0.0.158 C-LST: 10.0.0.216 100.0.0.155 
          RD: 10.0.0.64:8 auto-discovery 1119 0000:0000:0000:0000:0000
                                 2002::64              -       100     0       65000 i Or-ID: 10.0.0.64 C-LST: 10.0.0.216 100.0.0.155 
          RD: 100.0.0.162:1119 auto-discovery 1119 0000:0000:0000:0000:0000
                                 1001::162             -       100     0       65000 i Or-ID: 100.0.0.162 C-LST: 10.0.0.216 100.0.0.155 
          RD: 10.0.0.64:9 auto-discovery 1120 0000:0000:0000:0000:0000
                                 2002::64              -       100     0       65000 i Or-ID: 10.0.0.64 C-LST: 10.0.0.216 100.0.0.155 
          RD: 100.0.0.169:1120 auto-discovery 1120 0000:0000:0000:0000:0000
                                 2002::169             -       100     0       65000 i Or-ID: 100.0.0.169 C-LST: 10.0.0.216 100.0.0.155 
          RD: 0.0.1.136:1 auto-discovery 1121 0000:0000:0000:0000:0000
                                 2002::188             -       0       0       65000 i Or-ID: 100.0.0.188 C-LST: 10.0.0.216 100.0.0.155 
          RD: 10.0.0.64:10 auto-discovery 1121 0000:0000:0000:0000:0000
                                 2002::64              -       100     0       65000 i Or-ID: 10.0.0.64 C-LST: 10.0.0.216 100.0.0.155 
          RD: 10.0.0.64:11 auto-discovery 1122 0000:0000:0000:0000:0000
                                 2002::64              -       100     0       65000 i Or-ID: 10.0.0.64 C-LST: 10.0.0.216 100.0.0.155 
          RD: 10.0.0.216:1122 auto-discovery 1122 0000:0000:0000:0000:0000
                                 2002::216             -       100     0       i
          RD: 10.0.0.64:12 auto-discovery 1123 0000:0000:0000:0000:0000
                                 2002::64              -       100     0       65000 i Or-ID: 10.0.0.64 C-LST: 10.0.0.216 100.0.0.155 
          RD: 10.0.0.218:1123 auto-discovery 1123 0000:0000:0000:0000:0000
                                 2002::218             -       100     0       65000 i Or-ID: 10.0.0.218 C-LST: 10.0.0.216 100.0.0.155 
          RD: 1213:88 auto-discovery 1213 0000:0000:0000:0000:0000
                                 2002::88              0       100     0       65000 ? Or-ID: 100.0.0.88 C-LST: 10.0.0.216 100.0.0.155 
          RD: 10.0.0.74:2 auto-discovery 1213 0000:0000:0000:0000:0000
                                 2002::74              -       100     0       65000 i Or-ID: 10.0.0.74 C-LST: 10.0.0.216 100.0.0.155 
          RD: 1214:119 auto-discovery 1214 0000:0000:0000:0000:0000
                                 1001::119             0       100     0       65000 i Or-ID: 100.0.0.119 C-LST: 10.0.0.216 100.0.0.155 
          RD: 10.0.0.74:3 auto-discovery 1214 0000:0000:0000:0000:0000
                                 2002::74              -       100     0       65000 i Or-ID: 10.0.0.74 C-LST: 10.0.0.216 100.0.0.155 
          RD: 1215:122 auto-discovery 1215 0000:0000:0000:0000:0000
                                 2002::122             0       100     0       65000 i Or-ID: 100.0.0.122 C-LST: 10.0.0.216 100.0.0.155 
          RD: 10.0.0.74:4 auto-discovery 1215 0000:0000:0000:0000:0000
                                 2002::74              -       100     0       65000 i Or-ID: 10.0.0.74 C-LST: 10.0.0.216 100.0.0.155 
          RD: 1216:125 auto-discovery 1216 0000:0000:0000:0000:0000
                                 2002::125             -       100     0       65000 i Or-ID: 100.0.0.125 C-LST: 10.0.0.216 100.0.0.155 
          RD: 10.0.0.74:5 auto-discovery 1216 0000:0000:0000:0000:0000
                                 2002::74              -       100     0       65000 i Or-ID: 10.0.0.74 C-LST: 10.0.0.216 100.0.0.155 
          RD: 1217:130 auto-discovery 1217 0000:0000:0000:0000:0000
                                 2002::130             -       100     0       65000 i Or-ID: 100.0.0.130 C-LST: 10.0.0.216 100.0.0.155 
          RD: 10.0.0.74:6 auto-discovery 1217 0000:0000:0000:0000:0000
                                 2002::74              -       100     0       65000 i Or-ID: 10.0.0.74 C-LST: 10.0.0.216 100.0.0.155 
          RD: 10.0.0.74:7 auto-discovery 1218 0000:0000:0000:0000:0000
                                 2002::74              -       100     0       65000 i Or-ID: 10.0.0.74 C-LST: 10.0.0.216 100.0.0.155 
          RD: 100.0.0.158:1218 auto-discovery 1218 0000:0000:0000:0000:0000
                                 1001::158             -       100     0       65000 i Or-ID: 100.0.0.158 C-LST: 10.0.0.216 100.0.0.155 
          RD: 10.0.0.74:8 auto-discovery 1219 0000:0000:0000:0000:0000
                                 2002::74              -       100     0       65000 i Or-ID: 10.0.0.74 C-LST: 10.0.0.216 100.0.0.155 
          RD: 100.0.0.162:1219 auto-discovery 1219 0000:0000:0000:0000:0000
                                 1001::162             -       100     0       65000 i Or-ID: 100.0.0.162 C-LST: 10.0.0.216 100.0.0.155 
          RD: 10.0.0.74:9 auto-discovery 1220 0000:0000:0000:0000:0000
                                 2002::74              -       100     0       65000 i Or-ID: 10.0.0.74 C-LST: 10.0.0.216 100.0.0.155 
          RD: 100.0.0.169:1220 auto-discovery 1220 0000:0000:0000:0000:0000
                                 2002::169             -       100     0       65000 i Or-ID: 100.0.0.169 C-LST: 10.0.0.216 100.0.0.155 
          RD: 0.0.1.136:2 auto-discovery 1221 0000:0000:0000:0000:0000
                                 2002::188             -       0       0       65000 i Or-ID: 100.0.0.188 C-LST: 10.0.0.216 100.0.0.155 
          RD: 10.0.0.74:10 auto-discovery 1221 0000:0000:0000:0000:0000
                                 2002::74              -       100     0       65000 i Or-ID: 10.0.0.74 C-LST: 10.0.0.216 100.0.0.155 
          RD: 10.0.0.74:11 auto-discovery 1222 0000:0000:0000:0000:0000
                                 2002::74              -       100     0       65000 i Or-ID: 10.0.0.74 C-LST: 10.0.0.216 100.0.0.155 
          RD: 10.0.0.216:1222 auto-discovery 1222 0000:0000:0000:0000:0000
                                 2002::216             -       100     0       i
          RD: 10.0.0.74:12 auto-discovery 1223 0000:0000:0000:0000:0000
                                 2002::74              -       100     0       65000 i Or-ID: 10.0.0.74 C-LST: 10.0.0.216 100.0.0.155 
          RD: 10.0.0.218:1223 auto-discovery 1223 0000:0000:0000:0000:0000
                                 2002::218             -       100     0       65000 i Or-ID: 10.0.0.218 C-LST: 10.0.0.216 100.0.0.155 
          RD: 1314:88 auto-discovery 1314 0000:0000:0000:0000:0000
                                 2002::88              0       100     0       65000 ? Or-ID: 100.0.0.88 C-LST: 10.0.0.216 100.0.0.155 
          RD: 1314:119 auto-discovery 1314 0000:0000:0000:0000:0000
                                 1001::119             0       100     0       65000 i Or-ID: 100.0.0.119 C-LST: 10.0.0.216 100.0.0.155 
          RD: 1315:88 auto-discovery 1315 0000:0000:0000:0000:0000
                                 2002::88              0       100     0       65000 ? Or-ID: 100.0.0.88 C-LST: 10.0.0.216 100.0.0.155 
          RD: 1315:122 auto-discovery 1315 0000:0000:0000:0000:0000
                                 2002::122             0       100     0       65000 i Or-ID: 100.0.0.122 C-LST: 10.0.0.216 100.0.0.155 
          RD: 1316:88 auto-discovery 1316 0000:0000:0000:0000:0000
                                 2002::88              0       100     0       65000 ? Or-ID: 100.0.0.88 C-LST: 10.0.0.216 100.0.0.155 
          RD: 1316:125 auto-discovery 1316 0000:0000:0000:0000:0000
                                 2002::125             -       100     0       65000 i Or-ID: 100.0.0.125 C-LST: 10.0.0.216 100.0.0.155 
          RD: 1317:88 auto-discovery 1317 0000:0000:0000:0000:0000
                                 2002::88              0       100     0       65000 ? Or-ID: 100.0.0.88 C-LST: 10.0.0.216 100.0.0.155 
          RD: 1317:130 auto-discovery 1317 0000:0000:0000:0000:0000
                                 2002::130             -       100     0       65000 i Or-ID: 100.0.0.130 C-LST: 10.0.0.216 100.0.0.155 
          RD: 1318:88 auto-discovery 1318 0000:0000:0000:0000:0000
                                 2002::88              0       100     0       65000 ? Or-ID: 100.0.0.88 C-LST: 10.0.0.216 100.0.0.155 
          RD: 100.0.0.158:1318 auto-discovery 1318 0000:0000:0000:0000:0000
                                 1001::158             -       100     0       65000 i Or-ID: 100.0.0.158 C-LST: 10.0.0.216 100.0.0.155 
          RD: 1319:88 auto-discovery 1319 0000:0000:0000:0000:0000
                                 2002::88              0       100     0       65000 ? Or-ID: 100.0.0.88 C-LST: 10.0.0.216 100.0.0.155 
          RD: 100.0.0.162:1319 auto-discovery 1319 0000:0000:0000:0000:0000
                                 1001::162             -       100     0       65000 i Or-ID: 100.0.0.162 C-LST: 10.0.0.216 100.0.0.155 
          RD: 1320:88 auto-discovery 1320 0000:0000:0000:0000:0000
                                 2002::88              0       100     0       65000 ? Or-ID: 100.0.0.88 C-LST: 10.0.0.216 100.0.0.155 
          RD: 100.0.0.169:1320 auto-discovery 1320 0000:0000:0000:0000:0000
                                 2002::169             -       100     0       65000 i Or-ID: 100.0.0.169 C-LST: 10.0.0.216 100.0.0.155 
          RD: 1321:88 auto-discovery 1321 0000:0000:0000:0000:0000
                                 2002::88              0       100     0       65000 ? Or-ID: 100.0.0.88 C-LST: 10.0.0.216 100.0.0.155 
          RD: 0.0.1.136:3 auto-discovery 1321 0000:0000:0000:0000:0000
                                 2002::188             -       0       0       65000 i Or-ID: 100.0.0.188 C-LST: 10.0.0.216 100.0.0.155 
          RD: 1322:88 auto-discovery 1322 0000:0000:0000:0000:0000
                                 2002::88              0       100     0       65000 ? Or-ID: 100.0.0.88 C-LST: 10.0.0.216 100.0.0.155 
          RD: 10.0.0.216:1322 auto-discovery 1322 0000:0000:0000:0000:0000
                                 2002::216             -       100     0       i
          RD: 1323:88 auto-discovery 1323 0000:0000:0000:0000:0000
                                 2002::88              0       100     0       65000 ? Or-ID: 100.0.0.88 C-LST: 10.0.0.216 100.0.0.155 
          RD: 10.0.0.218:1323 auto-discovery 1323 0000:0000:0000:0000:0000
                                 2002::218             -       100     0       65000 i Or-ID: 10.0.0.218 C-LST: 10.0.0.216 100.0.0.155 
          RD: 1415:119 auto-discovery 1415 0000:0000:0000:0000:0000
                                 1001::119             0       100     0       65000 i Or-ID: 100.0.0.119 C-LST: 10.0.0.216 100.0.0.155 
          RD: 1415:122 auto-discovery 1415 0000:0000:0000:0000:0000
                                 2002::122             0       100     0       65000 i Or-ID: 100.0.0.122 C-LST: 10.0.0.216 100.0.0.155 
          RD: 1416:119 auto-discovery 1416 0000:0000:0000:0000:0000
                                 1001::119             0       100     0       65000 i Or-ID: 100.0.0.119 C-LST: 10.0.0.216 100.0.0.155 
          RD: 1416:125 auto-discovery 1416 0000:0000:0000:0000:0000
                                 2002::125             -       100     0       65000 i Or-ID: 100.0.0.125 C-LST: 10.0.0.216 100.0.0.155 
          RD: 1417:119 auto-discovery 1417 0000:0000:0000:0000:0000
                                 1001::119             0       100     0       65000 i Or-ID: 100.0.0.119 C-LST: 10.0.0.216 100.0.0.155 
          RD: 1417:130 auto-discovery 1417 0000:0000:0000:0000:0000
                                 2002::130             -       100     0       65000 i Or-ID: 100.0.0.130 C-LST: 10.0.0.216 100.0.0.155 
          RD: 1418:119 auto-discovery 1418 0000:0000:0000:0000:0000
                                 1001::119             0       100     0       65000 i Or-ID: 100.0.0.119 C-LST: 10.0.0.216 100.0.0.155 
          RD: 100.0.0.158:1418 auto-discovery 1418 0000:0000:0000:0000:0000
                                 1001::158             -       100     0       65000 i Or-ID: 100.0.0.158 C-LST: 10.0.0.216 100.0.0.155 
          RD: 1419:119 auto-discovery 1419 0000:0000:0000:0000:0000
                                 1001::119             0       100     0       65000 i Or-ID: 100.0.0.119 C-LST: 10.0.0.216 100.0.0.155 
          RD: 100.0.0.162:1419 auto-discovery 1419 0000:0000:0000:0000:0000
                                 1001::162             -       100     0       65000 i Or-ID: 100.0.0.162 C-LST: 10.0.0.216 100.0.0.155 
          RD: 1420:119 auto-discovery 1420 0000:0000:0000:0000:0000
                                 1001::119             0       100     0       65000 i Or-ID: 100.0.0.119 C-LST: 10.0.0.216 100.0.0.155 
          RD: 100.0.0.169:1420 auto-discovery 1420 0000:0000:0000:0000:0000
                                 2002::169             -       100     0       65000 i Or-ID: 100.0.0.169 C-LST: 10.0.0.216 100.0.0.155 
          RD: 1421:119 auto-discovery 1421 0000:0000:0000:0000:0000
                                 1001::119             0       100     0       65000 i Or-ID: 100.0.0.119 C-LST: 10.0.0.216 100.0.0.155 
          RD: 0.0.1.136:4 auto-discovery 1421 0000:0000:0000:0000:0000
                                 2002::188             -       0       0       65000 i Or-ID: 100.0.0.188 C-LST: 10.0.0.216 100.0.0.155 
          RD: 1422:119 auto-discovery 1422 0000:0000:0000:0000:0000
                                 1001::119             0       100     0       65000 i Or-ID: 100.0.0.119 C-LST: 10.0.0.216 100.0.0.155 
          RD: 10.0.0.216:1422 auto-discovery 1422 0000:0000:0000:0000:0000
                                 2002::216             -       100     0       i
          RD: 1423:119 auto-discovery 1423 0000:0000:0000:0000:0000
                                 1001::119             0       100     0       65000 i Or-ID: 100.0.0.119 C-LST: 10.0.0.216 100.0.0.155 
          RD: 10.0.0.218:1423 auto-discovery 1423 0000:0000:0000:0000:0000
                                 2002::218             -       100     0       65000 i Or-ID: 10.0.0.218 C-LST: 10.0.0.216 100.0.0.155 
          RD: 1516:122 auto-discovery 1516 0000:0000:0000:0000:0000
                                 2002::122             0       100     0       65000 i Or-ID: 100.0.0.122 C-LST: 10.0.0.216 100.0.0.155 
          RD: 1516:125 auto-discovery 1516 0000:0000:0000:0000:0000
                                 2002::125             -       100     0       65000 i Or-ID: 100.0.0.125 C-LST: 10.0.0.216 100.0.0.155 
          RD: 1517:122 auto-discovery 1517 0000:0000:0000:0000:0000
                                 2002::122             0       100     0       65000 i Or-ID: 100.0.0.122 C-LST: 10.0.0.216 100.0.0.155 
          RD: 1517:130 auto-discovery 1517 0000:0000:0000:0000:0000
                                 2002::130             -       100     0       65000 i Or-ID: 100.0.0.130 C-LST: 10.0.0.216 100.0.0.155 
          RD: 1518:122 auto-discovery 1518 0000:0000:0000:0000:0000
                                 2002::122             0       100     0       65000 i Or-ID: 100.0.0.122 C-LST: 10.0.0.216 100.0.0.155 
          RD: 100.0.0.158:1518 auto-discovery 1518 0000:0000:0000:0000:0000
                                 1001::158             -       100     0       65000 i Or-ID: 100.0.0.158 C-LST: 10.0.0.216 100.0.0.155 
          RD: 1519:122 auto-discovery 1519 0000:0000:0000:0000:0000
                                 2002::122             0       100     0       65000 i Or-ID: 100.0.0.122 C-LST: 10.0.0.216 100.0.0.155 
          RD: 100.0.0.162:1519 auto-discovery 1519 0000:0000:0000:0000:0000
                                 1001::162             -       100     0       65000 i Or-ID: 100.0.0.162 C-LST: 10.0.0.216 100.0.0.155 
          RD: 1520:122 auto-discovery 1520 0000:0000:0000:0000:0000
                                 2002::122             0       100     0       65000 i Or-ID: 100.0.0.122 C-LST: 10.0.0.216 100.0.0.155 
          RD: 100.0.0.169:1520 auto-discovery 1520 0000:0000:0000:0000:0000
                                 2002::169             -       100     0       65000 i Or-ID: 100.0.0.169 C-LST: 10.0.0.216 100.0.0.155 
          RD: 1521:122 auto-discovery 1521 0000:0000:0000:0000:0000
                                 2002::122             0       100     0       65000 i Or-ID: 100.0.0.122 C-LST: 10.0.0.216 100.0.0.155 
          RD: 0.0.1.136:5 auto-discovery 1521 0000:0000:0000:0000:0000
                                 2002::188             -       0       0       65000 i Or-ID: 100.0.0.188 C-LST: 10.0.0.216 100.0.0.155 
          RD: 1522:122 auto-discovery 1522 0000:0000:0000:0000:0000
                                 2002::122             0       100     0       65000 i Or-ID: 100.0.0.122 C-LST: 10.0.0.216 100.0.0.155 
          RD: 10.0.0.216:1522 auto-discovery 1522 0000:0000:0000:0000:0000
                                 2002::216             -       100     0       i
          RD: 1522:123 auto-discovery 1523 0000:0000:0000:0000:0000
                                 2002::122             0       100     0       65000 i Or-ID: 100.0.0.122 C-LST: 10.0.0.216 100.0.0.155 
          RD: 10.0.0.218:1523 auto-discovery 1523 0000:0000:0000:0000:0000
                                 2002::218             -       100     0       65000 i Or-ID: 10.0.0.218 C-LST: 10.0.0.216 100.0.0.155 
          RD: 1617:125 auto-discovery 1617 0000:0000:0000:0000:0000
                                 2002::125             -       100     0       65000 i Or-ID: 100.0.0.125 C-LST: 10.0.0.216 100.0.0.155 
          RD: 1617:130 auto-discovery 1617 0000:0000:0000:0000:0000
                                 2002::130             -       100     0       65000 i Or-ID: 100.0.0.130 C-LST: 10.0.0.216 100.0.0.155 
          RD: 1618:125 auto-discovery 1618 0000:0000:0000:0000:0000
                                 2002::125             -       100     0       65000 i Or-ID: 100.0.0.125 C-LST: 10.0.0.216 100.0.0.155 
          RD: 100.0.0.158:1618 auto-discovery 1618 0000:0000:0000:0000:0000
                                 1001::158             -       100     0       65000 i Or-ID: 100.0.0.158 C-LST: 10.0.0.216 100.0.0.155 
          RD: 1619:125 auto-discovery 1619 0000:0000:0000:0000:0000
                                 2002::125             -       100     0       65000 i Or-ID: 100.0.0.125 C-LST: 10.0.0.216 100.0.0.155 
          RD: 100.0.0.162:1619 auto-discovery 1619 0000:0000:0000:0000:0000
                                 1001::162             -       100     0       65000 i Or-ID: 100.0.0.162 C-LST: 10.0.0.216 100.0.0.155 
          RD: 1620:125 auto-discovery 1620 0000:0000:0000:0000:0000
                                 2002::125             -       100     0       65000 i Or-ID: 100.0.0.125 C-LST: 10.0.0.216 100.0.0.155 
          RD: 100.0.0.169:1620 auto-discovery 1620 0000:0000:0000:0000:0000
                                 2002::169             -       100     0       65000 i Or-ID: 100.0.0.169 C-LST: 10.0.0.216 100.0.0.155 
          RD: 1621:125 auto-discovery 1621 0000:0000:0000:0000:0000
                                 2002::125             -       100     0       65000 i Or-ID: 100.0.0.125 C-LST: 10.0.0.216 100.0.0.155 
          RD: 0.0.1.136:6 auto-discovery 1621 0000:0000:0000:0000:0000
                                 2002::188             -       0       0       65000 i Or-ID: 100.0.0.188 C-LST: 10.0.0.216 100.0.0.155 
          RD: 1622:125 auto-discovery 1622 0000:0000:0000:0000:0000
                                 2002::125             -       100     0       65000 i Or-ID: 100.0.0.125 C-LST: 10.0.0.216 100.0.0.155 
          RD: 10.0.0.216:1622 auto-discovery 1622 0000:0000:0000:0000:0000
                                 2002::216             -       100     0       i
          RD: 1623:125 auto-discovery 1623 0000:0000:0000:0000:0000
                                 2002::125             -       100     0       65000 i Or-ID: 100.0.0.125 C-LST: 10.0.0.216 100.0.0.155 
          RD: 10.0.0.218:1623 auto-discovery 1623 0000:0000:0000:0000:0000
                                 2002::218             -       100     0       65000 i Or-ID: 10.0.0.218 C-LST: 10.0.0.216 100.0.0.155 
          RD: 1718:130 auto-discovery 1718 0000:0000:0000:0000:0000
                                 2002::130             -       100     0       65000 i Or-ID: 100.0.0.130 C-LST: 10.0.0.216 100.0.0.155 
          RD: 100.0.0.158:1718 auto-discovery 1718 0000:0000:0000:0000:0000
                                 1001::158             -       100     0       65000 i Or-ID: 100.0.0.158 C-LST: 10.0.0.216 100.0.0.155 
          RD: 1719:130 auto-discovery 1719 0000:0000:0000:0000:0000
                                 2002::130             -       100     0       65000 i Or-ID: 100.0.0.130 C-LST: 10.0.0.216 100.0.0.155 
          RD: 100.0.0.162:1719 auto-discovery 1719 0000:0000:0000:0000:0000
                                 1001::162             -       100     0       65000 i Or-ID: 100.0.0.162 C-LST: 10.0.0.216 100.0.0.155 
          RD: 1720:130 auto-discovery 1720 0000:0000:0000:0000:0000
                                 2002::130             -       100     0       65000 i Or-ID: 100.0.0.130 C-LST: 10.0.0.216 100.0.0.155 
          RD: 100.0.0.169:1720 auto-discovery 1720 0000:0000:0000:0000:0000
                                 2002::169             -       100     0       65000 i Or-ID: 100.0.0.169 C-LST: 10.0.0.216 100.0.0.155 
          RD: 1721:130 auto-discovery 1721 0000:0000:0000:0000:0000
                                 2002::130             -       100     0       65000 i Or-ID: 100.0.0.130 C-LST: 10.0.0.216 100.0.0.155 
          RD: 0.0.1.136:7 auto-discovery 1721 0000:0000:0000:0000:0000
                                 2002::188             -       0       0       65000 i Or-ID: 100.0.0.188 C-LST: 10.0.0.216 100.0.0.155 
          RD: 1722:130 auto-discovery 1722 0000:0000:0000:0000:0000
                                 2002::130             -       100     0       65000 i Or-ID: 100.0.0.130 C-LST: 10.0.0.216 100.0.0.155 
          RD: 10.0.0.216:1722 auto-discovery 1722 0000:0000:0000:0000:0000
                                 2002::216             -       100     0       i
          RD: 1723:130 auto-discovery 1723 0000:0000:0000:0000:0000
                                 2002::130             -       100     0       65000 i Or-ID: 100.0.0.130 C-LST: 10.0.0.216 100.0.0.155 
          RD: 10.0.0.218:1723 auto-discovery 1723 0000:0000:0000:0000:0000
                                 2002::218             -       100     0       65000 i Or-ID: 10.0.0.218 C-LST: 10.0.0.216 100.0.0.155 
          RD: 100.0.0.158:1819 auto-discovery 1819 0000:0000:0000:0000:0000
                                 1001::158             -       100     0       65000 i Or-ID: 100.0.0.158 C-LST: 10.0.0.216 100.0.0.155 
          RD: 100.0.0.162:1819 auto-discovery 1819 0000:0000:0000:0000:0000
                                 1001::162             -       100     0       65000 i Or-ID: 100.0.0.162 C-LST: 10.0.0.216 100.0.0.155 
          RD: 100.0.0.158:1820 auto-discovery 1820 0000:0000:0000:0000:0000
                                 1001::158             -       100     0       65000 i Or-ID: 100.0.0.158 C-LST: 10.0.0.216 100.0.0.155 
          RD: 100.0.0.169:1820 auto-discovery 1820 0000:0000:0000:0000:0000
                                 2002::169             -       100     0       65000 i Or-ID: 100.0.0.169 C-LST: 10.0.0.216 100.0.0.155 
          RD: 0.0.1.136:8 auto-discovery 1821 0000:0000:0000:0000:0000
                                 2002::188             -       0       0       65000 i Or-ID: 100.0.0.188 C-LST: 10.0.0.216 100.0.0.155 
          RD: 100.0.0.158:1821 auto-discovery 1821 0000:0000:0000:0000:0000
                                 1001::158             -       100     0       65000 i Or-ID: 100.0.0.158 C-LST: 10.0.0.216 100.0.0.155 
          RD: 10.0.0.216:1822 auto-discovery 1822 0000:0000:0000:0000:0000
                                 2002::216             -       100     0       i
          RD: 100.0.0.158:1822 auto-discovery 1822 0000:0000:0000:0000:0000
                                 1001::158             -       100     0       65000 i Or-ID: 100.0.0.158 C-LST: 10.0.0.216 100.0.0.155 
          RD: 10.0.0.218:1823 auto-discovery 1823 0000:0000:0000:0000:0000
                                 2002::218             -       100     0       65000 i Or-ID: 10.0.0.218 C-LST: 10.0.0.216 100.0.0.155 
          RD: 100.0.0.158:1823 auto-discovery 1823 0000:0000:0000:0000:0000
                                 1001::158             -       100     0       65000 i Or-ID: 100.0.0.158 C-LST: 10.0.0.216 100.0.0.155 
          RD: 100.0.0.162:1920 auto-discovery 1920 0000:0000:0000:0000:0000
                                 1001::162             -       100     0       65000 i Or-ID: 100.0.0.162 C-LST: 10.0.0.216 100.0.0.155 
          RD: 100.0.0.169:1920 auto-discovery 1920 0000:0000:0000:0000:0000
                                 2002::169             -       100     0       65000 i Or-ID: 100.0.0.169 C-LST: 10.0.0.216 100.0.0.155 
          RD: 0.0.1.136:9 auto-discovery 1921 0000:0000:0000:0000:0000
                                 2002::188             -       0       0       65000 i Or-ID: 100.0.0.188 C-LST: 10.0.0.216 100.0.0.155 
          RD: 100.0.0.162:1921 auto-discovery 1921 0000:0000:0000:0000:0000
                                 1001::162             -       100     0       65000 i Or-ID: 100.0.0.162 C-LST: 10.0.0.216 100.0.0.155 
          RD: 10.0.0.216:1922 auto-discovery 1922 0000:0000:0000:0000:0000
                                 2002::216             -       100     0       i
          RD: 100.0.0.162:1922 auto-discovery 1922 0000:0000:0000:0000:0000
                                 1001::162             -       100     0       65000 i Or-ID: 100.0.0.162 C-LST: 10.0.0.216 100.0.0.155 
          RD: 10.0.0.218:1923 auto-discovery 1923 0000:0000:0000:0000:0000
                                 2002::218             -       100     0       65000 i Or-ID: 10.0.0.218 C-LST: 10.0.0.216 100.0.0.155 
          RD: 100.0.0.162:1923 auto-discovery 1923 0000:0000:0000:0000:0000
                                 1001::162             -       100     0       65000 i Or-ID: 100.0.0.162 C-LST: 10.0.0.216 100.0.0.155 
          RD: 0.0.1.136:10 auto-discovery 2021 0000:0000:0000:0000:0000
                                 2002::188             -       0       0       65000 i Or-ID: 100.0.0.188 C-LST: 10.0.0.216 100.0.0.155 
          RD: 100.0.0.169:2021 auto-discovery 2021 0000:0000:0000:0000:0000
                                 2002::169             -       100     0       65000 i Or-ID: 100.0.0.169 C-LST: 10.0.0.216 100.0.0.155 
          RD: 10.0.0.216:2022 auto-discovery 2022 0000:0000:0000:0000:0000
                                 2002::216             -       100     0       i
          RD: 100.0.0.169:2022 auto-discovery 2022 0000:0000:0000:0000:0000
                                 2002::169             -       100     0       65000 i Or-ID: 100.0.0.169 C-LST: 10.0.0.216 100.0.0.155 
          RD: 10.0.0.218:2023 auto-discovery 2023 0000:0000:0000:0000:0000
                                 2002::218             -       100     0       65000 i Or-ID: 10.0.0.218 C-LST: 10.0.0.216 100.0.0.155 
          RD: 100.0.0.169:2023 auto-discovery 2023 0000:0000:0000:0000:0000
                                 2002::169             -       100     0       65000 i Or-ID: 100.0.0.169 C-LST: 10.0.0.216 100.0.0.155 
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
          RD: 0.0.1.136:11 auto-discovery 2122 0000:0000:0000:0000:0000
                                 2002::188             -       0       0       65000 i Or-ID: 100.0.0.188 C-LST: 10.0.0.216 100.0.0.155 
          RD: 10.0.0.216:2122 auto-discovery 2122 0000:0000:0000:0000:0000
                                 2002::216             -       100     0       i
          RD: 0.0.1.136:12 auto-discovery 2123 0000:0000:0000:0000:0000
                                 2002::188             -       0       0       65000 i Or-ID: 100.0.0.188 C-LST: 10.0.0.216 100.0.0.155 
          RD: 10.0.0.218:2123 auto-discovery 2123 0000:0000:0000:0000:0000
                                 2002::218             -       100     0       65000 i Or-ID: 10.0.0.218 C-LST: 10.0.0.216 100.0.0.155 
          RD: 10.0.0.216:2223 auto-discovery 2223 0000:0000:0000:0000:0000
                                 2002::216             -       100     0       i
          RD: 10.0.0.218:2223 auto-discovery 2223 0000:0000:0000:0000:0000
                                 2002::218             -       100     0       65000 i Or-ID: 10.0.0.218 C-LST: 10.0.0.216 100.0.0.155 
 * >Ec    RD: 10.0.0.214:84 auto-discovery 6214 0000:0000:0000:0000:0000
                                 10.0.0.214            -       100     0       i Or-ID: 10.0.0.214 C-LST: 10.0.0.216 
 *  ec    RD: 10.0.0.214:84 auto-discovery 6214 0000:0000:0000:0000:0000
                                 10.0.0.214            -       100     0       i Or-ID: 10.0.0.214 C-LST: 10.0.1.156 
          RD: 50:88 imet 100.0.0.88
                                 2002::88              0       100     0       65000 ? Or-ID: 100.0.0.88 C-LST: 10.0.0.216 100.0.0.155 
          RD: 50:119 imet 100.0.0.119
                                 1001::119             0       100     0       65000 i Or-ID: 100.0.0.119 C-LST: 10.0.0.216 100.0.0.155 
          RD: 50:122 imet 100.0.0.122
                                 2002::122             0       100     0       65000 i Or-ID: 100.0.0.122 C-LST: 10.0.0.216 100.0.0.155 
          RD: 100.0.0.158:50 imet 1001::158
                                 1001::158             -       100     0       65000 i Or-ID: 100.0.0.158 C-LST: 10.0.0.216 100.0.0.155 
          RD: 100.0.0.162:50 imet 1001::162
                                 1001::162             -       100     0       65000 i Or-ID: 100.0.0.162 C-LST: 10.0.0.216 100.0.0.155 
          RD: 100.0.0.169:50 imet 2002::169
                                 2002::169             -       100     0       65000 i Or-ID: 100.0.0.169 C-LST: 10.0.0.216 100.0.0.155 
          RD: 10.0.0.216:50 imet 2002::216
                                 2002::216             -       100     0       i
          RD: 10.0.0.218:50 imet 2002::218
                                 2002::218             -       100     0       65000 i Or-ID: 10.0.0.218 C-LST: 10.0.0.216 100.0.0.155 
          RD: 40:41 ip-prefix 40.41.190.0/24
                                 1001::41              -       100     0       65000 i Or-ID: 100.0.0.41 C-LST: 10.0.0.216 100.0.0.155 
          RD: 40:42 ip-prefix 40.42.190.0/24
                                 2002::42              -       100     0       65000 i Or-ID: 100.0.0.42 C-LST: 10.0.0.216 100.0.0.155 
          RD: 40:119 ip-prefix 40.119.190.0/24
                                 1001::119             0       100     0       65000 ? Or-ID: 100.0.0.119 C-LST: 10.0.0.216 100.0.0.155 
          RD: 40:122 ip-prefix 40.122.190.0/24
                                 2002::122             0       100     0       65000 ? Or-ID: 100.0.0.122 C-LST: 10.0.0.216 100.0.0.155 
          RD: 40:125 ip-prefix 40.125.190.0/24
                                 2002::125             0       100     0       65000 ? Or-ID: 100.0.0.125 C-LST: 10.0.0.216 100.0.0.155 
          RD: 40:130 ip-prefix 40.130.190.0/24
                                 2002::130             0       100     0       65000 ? Or-ID: 100.0.0.130 C-LST: 10.0.0.216 100.0.0.155 
          RD: 100.0.0.158:40 ip-prefix 40.158.190.0/24
                                 1001::158             -       100     0       65000 i Or-ID: 100.0.0.158 C-LST: 10.0.0.216 100.0.0.155 
          RD: 100.0.0.162:40 ip-prefix 40.162.190.0/24
                                 1001::162             -       100     0       65000 i Or-ID: 100.0.0.162 C-LST: 10.0.0.216 100.0.0.155 
          RD: 100.0.0.169:40 ip-prefix 40.169.190.0/24
                                 2002::169             -       100     0       65000 i Or-ID: 100.0.0.169 C-LST: 10.0.0.216 100.0.0.155 
 * >      RD: 10.0.0.216:40 ip-prefix 40.190.216.0/24
                                 10.0.0.216            -       100     0       i
          RD: 10.0.0.218:40 ip-prefix 40.190.218.0/24
                                 2002::218             -       100     0       65000 i Or-ID: 10.0.0.218 C-LST: 10.0.0.216 100.0.0.155 
          RD: 42:119 ip-prefix 42.119.190.0/24
                                 1001::119             0       100     0       65000 ? Or-ID: 100.0.0.119 C-LST: 10.0.0.216 100.0.0.155 
          RD: 42:122 ip-prefix 42.122.190.0/24
                                 2002::122             0       100     0       65000 ? Or-ID: 100.0.0.122 C-LST: 10.0.0.216 100.0.0.155 
          RD: 42:125 ip-prefix 42.125.190.0/24
                                 2002::125             0       100     0       65000 ? Or-ID: 100.0.0.125 C-LST: 10.0.0.216 100.0.0.155 
          RD: 42:130 ip-prefix 42.130.190.0/24
                                 2002::130             0       100     0       65000 ? Or-ID: 100.0.0.130 C-LST: 10.0.0.216 100.0.0.155 
          RD: 100.0.0.158:42 ip-prefix 42.158.190.0/24
                                 1001::158             -       100     0       65000 i Or-ID: 100.0.0.158 C-LST: 10.0.0.216 100.0.0.155 
          RD: 100.0.0.162:42 ip-prefix 42.162.190.0/24
                                 1001::162             -       100     0       65000 i Or-ID: 100.0.0.162 C-LST: 10.0.0.216 100.0.0.155 
          RD: 100.0.0.169:42 ip-prefix 42.169.190.0/24
                                 2002::169             -       100     0       65000 i Or-ID: 100.0.0.169 C-LST: 10.0.0.216 100.0.0.155 
 * >      RD: 10.0.0.216:42 ip-prefix 42.190.216.0/24
                                 10.0.0.216            -       100     0       i
          RD: 10.0.0.218:42 ip-prefix 42.190.218.0/24
                                 2002::218             -       100     0       65000 i Or-ID: 10.0.0.218 C-LST: 10.0.0.216 100.0.0.155 
 * >Ec    RD: 54:7001 ip-prefix 50.10.54.0/24
                                 10.0.0.54             -       100     0       ? Or-ID: 10.0.0.54 C-LST: 10.0.0.216 
 *  ec    RD: 54:7001 ip-prefix 50.10.54.0/24
                                 10.0.0.54             -       100     0       ? Or-ID: 10.0.0.54 C-LST: 10.0.1.156 
          RD: 40:41 ip-prefix 2600:40:41:190::/64
                                 1001::41              -       100     0       65000 i Or-ID: 100.0.0.41 C-LST: 10.0.0.216 100.0.0.155 
          RD: 40:42 ip-prefix 2600:40:42:190::/64
                                 2002::42              -       100     0       65000 i Or-ID: 100.0.0.42 C-LST: 10.0.0.216 100.0.0.155 
          RD: 40:119 ip-prefix 2600:40:119:190::/64
                                 1001::119             0       100     0       65000 ? Or-ID: 100.0.0.119 C-LST: 10.0.0.216 100.0.0.155 
          RD: 40:122 ip-prefix 2600:40:122:190::/64
                                 2002::122             0       100     0       65000 ? Or-ID: 100.0.0.122 C-LST: 10.0.0.216 100.0.0.155 
          RD: 40:125 ip-prefix 2600:40:125:190::/64
                                 2002::125             0       100     0       65000 ? Or-ID: 100.0.0.125 C-LST: 10.0.0.216 100.0.0.155 
          RD: 40:130 ip-prefix 2600:40:130:190::/64
                                 2002::130             0       100     0       65000 ? Or-ID: 100.0.0.130 C-LST: 10.0.0.216 100.0.0.155 
          RD: 100.0.0.158:40 ip-prefix 2600:40:158:190::/64
                                 1001::158             -       100     0       65000 i Or-ID: 100.0.0.158 C-LST: 10.0.0.216 100.0.0.155 
          RD: 100.0.0.162:40 ip-prefix 2600:40:162:190::/64
                                 1001::162             -       100     0       65000 i Or-ID: 100.0.0.162 C-LST: 10.0.0.216 100.0.0.155 
          RD: 100.0.0.169:40 ip-prefix 2600:40:169:190::/64
                                 2002::169             -       100     0       65000 i Or-ID: 100.0.0.169 C-LST: 10.0.0.216 100.0.0.155 
 * >      RD: 10.0.0.216:40 ip-prefix 2600:40:190:216::/64
                                 10.0.0.216            -       100     0       i
          RD: 10.0.0.218:40 ip-prefix 2600:40:190:218::/64
                                 2002::218             -       100     0       65000 i Or-ID: 10.0.0.218 C-LST: 10.0.0.216 100.0.0.155 
          RD: 42:119 ip-prefix 2600:42:119:190::/64
                                 1001::119             0       100     0       65000 ? Or-ID: 100.0.0.119 C-LST: 10.0.0.216 100.0.0.155 
          RD: 42:122 ip-prefix 2600:42:122:190::/64
                                 2002::122             0       100     0       65000 ? Or-ID: 100.0.0.122 C-LST: 10.0.0.216 100.0.0.155 
          RD: 42:125 ip-prefix 2600:42:125:190::/64
                                 2002::125             0       100     0       65000 ? Or-ID: 100.0.0.125 C-LST: 10.0.0.216 100.0.0.155 
          RD: 42:130 ip-prefix 2600:42:130:190::/64
                                 2002::130             0       100     0       65000 ? Or-ID: 100.0.0.130 C-LST: 10.0.0.216 100.0.0.155 
          RD: 100.0.0.158:42 ip-prefix 2600:42:158:190::/64
                                 1001::158             -       100     0       65000 i Or-ID: 100.0.0.158 C-LST: 10.0.0.216 100.0.0.155 
          RD: 100.0.0.162:42 ip-prefix 2600:42:162:190::/64
                                 1001::162             -       100     0       65000 i Or-ID: 100.0.0.162 C-LST: 10.0.0.216 100.0.0.155 
          RD: 100.0.0.169:42 ip-prefix 2600:42:169:190::/64
                                 2002::169             -       100     0       65000 i Or-ID: 100.0.0.169 C-LST: 10.0.0.216 100.0.0.155 
 * >      RD: 10.0.0.216:42 ip-prefix 2600:42:190:216::/64
                                 10.0.0.216            -       100     0       i
          RD: 10.0.0.218:42 ip-prefix 2600:42:190:218::/64
                                 2002::218             -       100     0       65000 i Or-ID: 10.0.0.218 C-LST: 10.0.0.216 100.0.0.155 
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
 * >Ec    RD: 10000:128 IPv4 prefix 20.128.197.0/24
                                 10.0.0.128            0       100     0       ? Or-ID: 10.0.0.128 C-LST: 10.0.0.216 
 *  ec    RD: 10000:128 IPv4 prefix 20.128.197.0/24
                                 10.0.0.128            0       100     0       ? Or-ID: 10.0.0.128 C-LST: 10.0.1.156 
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
 * >Ec    RD: 120:7001 IPv4 prefix 50.10.120.0/24
                                 10.0.0.120            0       100     0       ? Or-ID: 10.0.0.120 C-LST: 10.0.0.216 
 *  ec    RD: 120:7001 IPv4 prefix 50.10.120.0/24
                                 10.0.0.120            0       100     0       ? Or-ID: 10.0.0.120 C-LST: 10.0.1.156 
 * >Ec    RD: 7001:128 IPv4 prefix 50.10.128.0/24
                                 10.0.0.128            0       100     0       ? Or-ID: 10.0.0.128 C-LST: 10.0.0.216 
 *  ec    RD: 7001:128 IPv4 prefix 50.10.128.0/24
                                 10.0.0.128            0       100     0       ? Or-ID: 10.0.0.128 C-LST: 10.0.1.156 
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
 * >Ec    RD: 214:7001 IPv4 prefix 50.10.214.0/24
                                 10.0.0.214            -       100     0       i Or-ID: 10.0.0.214 C-LST: 10.0.0.216 
 *  ec    RD: 214:7001 IPv4 prefix 50.10.214.0/24
                                 10.0.0.214            -       100     0       i Or-ID: 10.0.0.214 C-LST: 10.0.1.156 
 * >      RD: 216:7001 IPv4 prefix 50.10.216.0/24
                                 10.0.0.216            -       100     0       i
 * >      RD: 156:5001 IPv4 prefix 50.11.156.0/24
                                 10.0.1.156            -       100     0       i
 * >      RD: 5128:5128 IPv4 prefix 50.128.156.0/24
                                 10.0.1.156            -       100     0       i
 * >      RD: 5128:5128 IPv4 prefix 50.129.156.0/24
                                 10.0.1.156            -       100     0       i
 * >      RD: 5128:5128 IPv4 prefix 50.130.156.0/24
                                 10.0.1.156            -       100     0       i
 * >      RD: 10.0.0.216:128 IPv4 prefix 128.190.216.0/24
                                 10.0.0.216            -       100     0       i
 * >      RD: 10.0.0.216:129 IPv4 prefix 129.190.216.0/24
                                 10.0.0.216            -       100     0       i
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
  Connect timer is active, time left: 00:02:04
  Connection interval is 148 seconds
  Failed connection attempts is 2931
  Idle-restart timer is inactive
  BGP state is Active
  Number of transitions to established: 0
  Last state was Connect
  Last event was TransportError
  Last sent socket-error:Connect (Network is unreachable), Last time 00:00:43, First time 5d18h, Repeats 2930
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
  Last read 1d20h, last write 1d20h
  Hold time is 180, keepalive interval is 60 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is inactive
  Keepalive timer is inactive
  Connect timer is active, time left: 00:01:49
  Connection interval is 148 seconds
  Failed connection attempts is 3459
  Idle-restart timer is inactive
  BGP state is Active
  Number of transitions to established: 2
  Last state was Connect
  Last event was TransportError
  Last sent notification:Hold Timer Expired Error/None, Last time 1d20h
  Last sent socket-error:Connect (Network is unreachable), Last time 00:01:17, First time 1d20h, Repeats 550
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

BGP neighbor is 10.0.0.53, remote AS 64512, internal link
 Description: Arrcus-53
  BGP version 4, remote router ID 10.0.0.53, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 1d20h, last write 1d20h
  Hold time is 180, keepalive interval is 60 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is inactive
  Keepalive timer is inactive
  Connect timer is active, time left: 00:00:05
  Connection interval is 20 seconds
  Failed connection attempts is 6945
  Idle-restart timer is inactive
  BGP state is Connect
  Number of transitions to established: 5
  Last state was Active
  Last event was ConnectRetry
  Last sent notification:Hold Timer Expired Error/None, Last time 1d20h, First time 1d21h, Repeats 4
  Last sent socket-error:Connect (Network is unreachable), Last time 1d20h, First time 1d21h, Repeats 30
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
  Last read 1d22h, last write 1d20h
  Hold time is 180, keepalive interval is 60 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is inactive
  Keepalive timer is inactive
  Connect timer is active, time left: 00:00:02
  Connection interval is 20 seconds
  Failed connection attempts is 6949
  Idle-restart timer is inactive
  BGP state is Connect
  Number of transitions to established: 7
  Last state was Active
  Last event was ConnectRetry
  Last sent notification:Hold Timer Expired Error/None, Last time 1d22h, First time 5d01h, Repeats 2
  Last rcvd notification:Cease/other configuration change, Last time 2d01h, First time 5d17h, Repeats 3
  Last sent socket-error:Connect (Connection refused), Last time 1d20h
  Last rcvd socket-error:Connection reset by peer, Last time 1d20h, First time 4d20h, Repeats 4
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
  Last read 1d22h, last write 1d22h
  Hold time is 180, keepalive interval is 60 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is inactive
  Keepalive timer is inactive
  Connect timer is active, time left: 00:00:21
  Connection interval is 20 seconds
  Failed connection attempts is 2705
  Idle-restart timer is inactive
  BGP state is Connect
  Number of transitions to established: 9
  Last state was Active
  Last event was ConnectRetry
  Last sent notification:Hold Timer Expired Error/None, Last time 4d21h, First time 5d01h, Repeats 1
  Last rcvd notification:Cease/other configuration change, Last time 1d22h, First time 5d18h, Repeats 6
  Last sent socket-error:Connect (Network is unreachable), Last time 17:15:16, First time 1d22h, Repeats 72
  Last rcvd socket-error:Connection reset by peer, Last time 2d01h, First time 4d22h, Repeats 5
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
  Total Number of TCP retransmissions: 1
  Options:
    Timestamps enabled: no
    Selective Acknowledgments enabled: no
    Window Scale enabled: no
    Explicit Congestion Notification (ECN) enabled: no
  Socket Statistics:
    Window Scale (wscale): 0,0
    Retransmission Timeout (rto): 2000.0ms
    Round-trip Time (rtt/rtvar): 0.0ms/250.0ms
    Delayed Ack Timeout (ato): 0.0ms
    Congestion Window (cwnd): 1
    Slow-start Threshold (ssthresh): 7

BGP neighbor is 10.0.0.84, remote AS 64512, internal link
 Description: Ericsson_84
  BGP version 4, remote router ID 10.0.0.84, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 1d21h, last write 1d21h
  Hold time is 180, keepalive interval is 60 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is inactive
  Keepalive timer is inactive
  Connect timer is active, time left: 00:00:11
  Connection interval is 20 seconds
  Failed connection attempts is 6945
  Idle-restart timer is inactive
  BGP state is Connect
  Number of transitions to established: 1
  Last state was Active
  Last event was ConnectRetry
  Last sent notification:Hold Timer Expired Error/None, Last time 1d21h
  Last sent socket-error:Connect (Network is unreachable), Last time 1d20h, First time 1d21h, Repeats 27
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

BGP neighbor is 10.0.0.120, remote AS 64512, internal link
 Description: Huawei_120
  BGP version 4, remote router ID 10.0.0.120, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 1d20h, last write 1d20h
  Hold time is 180, keepalive interval is 60 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is inactive
  Keepalive timer is inactive
  Connect timer is active, time left: 00:00:02
  Connection interval is 20 seconds
  Failed connection attempts is 2727
  Idle-restart timer is inactive
  BGP state is Connect
  Number of transitions to established: 9
  Last state was Active
  Last event was ConnectRetry
  Last sent notification:Hold Timer Expired Error/None, Last time 1d20h, First time 1d20h, Repeats 1
  Last rcvd notification:Cease/connection collision resolution, Last time 1d21h
  Last sent socket-error:Connect (Network is unreachable), Last time 17:44:54, First time 1d20h, Repeats 14
  Last rcvd socket-error:Connection reset by peer, Last time 1d20h, First time 1d20h, Repeats 1
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
  Connect timer is active, time left: 00:01:45
  Connection interval is 148 seconds
  Failed connection attempts is 683
  Idle-restart timer is inactive
  BGP state is Active
  Number of transitions to established: 0
  Last state was Connect
  Last event was TransportError
  Last sent socket-error:Connect (Network is unreachable), Last time 00:00:48, First time 1d20h, Repeats 533
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
  Last read 5d00h, last write 5d00h
  Hold time is 180, keepalive interval is 60 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is inactive
  Keepalive timer is inactive
  Connect timer is active, time left: 00:00:18
  Connection interval is 20 seconds
  Failed connection attempts is 3310
  Idle-restart timer is inactive
  BGP state is Connect
  Number of transitions to established: 1
  Last state was Active
  Last event was ConnectRetry
  Last sent notification:Open Message Error/unsupported capability, Last time 5d00h, First time 5d00h, Repeats 38
    Sent data: 0x010400010080010400020080
  Last rcvd notification:Cease/peer de-configured, Last time 5d00h
  Last sent socket-error:Connect (Network is unreachable), Last time 1d03h, First time 1d20h, Repeats 7
  Last rcvd socket-error:Connection reset by peer, Last time 5d00h, First time 5d00h, Repeats 5
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

BGP neighbor is 10.0.0.131, remote AS 64512, internal link
 Description: Juniper-131-JCNR
  BGP version 4, remote router ID 10.0.0.131, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 1d01h, last write 1d01h
  Hold time is 90, keepalive interval is 30 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is inactive
  Keepalive timer is inactive
  Connect timer is active, time left: 00:01:19
  Connection interval is 148 seconds
  Failed connection attempts is 3449
  Idle-restart timer is inactive
  BGP state is Active
  Number of transitions to established: 2
  Last state was Connect
  Last event was TransportError
  Last sent notification:Hold Timer Expired Error/None, Last time 1d01h, First time 1d20h, Repeats 1
  Last rcvd notification:Cease/connection rejected, Last time 1d21h
  Last sent socket-error:Connect (Network is unreachable), Last time 00:01:43, First time 1d20h, Repeats 548
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
    Opens:                  4         4
    Notifications:          2         1
    Updates:              494         8
    Keepalives:         13177     12446
    Route Refresh:          0         0
    Total messages:     13677     12459
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

BGP neighbor is 10.0.0.156, remote AS 64512, internal link
 Description: Juniper-156
  BGP version 4, remote router ID 10.0.0.156, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 1d20h, last write 1d20h
  Hold time is 90, keepalive interval is 30 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is inactive
  Keepalive timer is inactive
  Connect timer is active, time left: 00:01:09
  Connection interval is 148 seconds
  Failed connection attempts is 56
  Idle-restart timer is inactive
  BGP state is Active
  Number of transitions to established: 4
  Last state was Connect
  Last event was TransportError
  Last sent notification:Hold Timer Expired Error/None, Last time 1d20h, First time 1d20h, Repeats 1
  Last rcvd notification:Cease/connection rejected, Last time 1d21h
  Last sent socket-error:Connect (Network is unreachable), Last time 00:01:26, First time 1d20h, Repeats 593
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
  Last read 1d01h, last write 1d01h
  Hold time is 90, keepalive interval is 30 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is inactive
  Keepalive timer is inactive
  Connect timer is active, time left: 00:01:30
  Connection interval is 148 seconds
  Failed connection attempts is 559
  Idle-restart timer is inactive
  BGP state is Active
  Number of transitions to established: 4
  Last state was Connect
  Last event was TransportError
  Last sent notification:Hold Timer Expired Error/None, Last time 1d01h, First time 2d01h, Repeats 2
  Last rcvd notification:Cease/connection rejected, Last time 1d21h
  Last sent socket-error:Connect (Network is unreachable), Last time 00:01:10, First time 1d20h, Repeats 546
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
    Opens:                339       339
    Notifications:        337         1
    Updates:              526        25
    Keepalives:         10901     10304
    Route Refresh:          0         2
    Total messages:     12103     10671
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
  Connect timer is active, time left: 00:00:31
  Connection interval is 148 seconds
  Failed connection attempts is 941
  Idle-restart timer is inactive
  BGP state is Active
  Number of transitions to established: 0
  Last state was Connect
  Last event was TransportError
  Last sent socket-error:Connect (Network is unreachable), Last time 00:02:10, First time 5d18h, Repeats 2935
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
  Last read 2d01h, last write 1d20h
  Hold time is 90, keepalive interval is 30 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is inactive
  Keepalive timer is inactive
  Connect timer is active, time left: 00:00:11
  Connection interval is 20 seconds
  Failed connection attempts is 2853
  Idle-restart timer is inactive
  BGP state is Connect
  Number of transitions to established: 1
  Last state was Active
  Last event was ConnectRetry
  Last rcvd notification:Cease/administrative shutdown, Last time 2d01h
  Last sent socket-error:Connect (Network is unreachable), Last time 18:13:23, First time 1d02h, Repeats 5
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

BGP neighbor is 10.0.0.216, remote AS 64512, internal link
 Description: 2-23-5G-NOKIA-216
  BGP version 4, remote router ID 10.0.0.216, VRF default
  Inherits configuration from and member of peer-group 2-23-5G-RR
  Last read 00:00:24, last write 00:00:22
  Hold time is 90, keepalive interval is 30 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:01:06
  Keepalive timer is active, time left: 00:00:05
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 1d19h
  Number of transitions to established: 4
  Last state was OpenConfirm
  Last event was RecvRtRefresh
  Last sent notification:Cease/other configuration change, Last time 1d20h
  Last rcvd notification:Cease/administrative reset, Last time 1d19h
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
      Received 1d19h
      Number of stale paths removed after graceful restart: 0
      Number of paths received before End-of-RIB: 4
    L2VPN EVPN End-of-RIB received: Yes
      Received 1d19h
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
    Updates:               72      3123
    Keepalives:          6214      5306
    Route Refresh:          0        11
    Total messages:      6291      8446
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    VPN-IPv4:                         2        14             14                   9
    IPv6 Unicast:                     0         0              0                   0
    EVPN:                             3       238             38                  32
  Configured maximum total number of routes is 256000, warning limit is 204800
  Inbound updates dropped by reason:
    AS path loop detection: 0
    Cluster ID loop detection: 5
    Enforced First AS: 0
    Malformed MPBGP routes: 1166
    Originator ID matches local router ID: 0
    Nexthop matches local IP address: 11
    Unexpected IPv6 nexthop for IPv4 routes: 0
    AS_SET/AS_CONFED_SET in AS_PATH for IPv4 Unicast: 0
    AS_SET/AS_CONFED_SET in AS_PATH for IPv6 Unicast: 0
  Inbound updates with attribute errors:
    Resulting in removal of all paths in update (treat as withdraw): 11
    Resulting in AFI/SAFI disable: 0
    Resulting in attribute ignore: 0
    Disabled AFI/SAFIs: None
    Last treat-as-withdraw attribute error: Nexthop is local address
    Last update with error received at: 01:11:07
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
  Total Number of TCP retransmissions: 82
  Options:
    Timestamps enabled: yes
    Selective Acknowledgments enabled: no
    Window Scale enabled: yes
    Explicit Congestion Notification (ECN) enabled: no
  Socket Statistics:
    Window Scale (wscale): 0,7
    Retransmission Timeout (rto): 204.0ms
    Round-trip Time (rtt/rtvar): 3.5ms/3.4ms
    Delayed Ack Timeout (ato): 40.0ms
    Congestion Window (cwnd): 2
    Slow-start Threshold (ssthresh): 2
    TCP Throughput: 4.58 Mbps
    Recv Round-trip Time (rcv_rtt): 2153.8ms
    Advertised Recv Window (rcv_space): 32958

BGP neighbor is 10.0.0.217, remote AS 64512, internal link
 Description: Nokia
  BGP version 4, remote router ID 10.0.0.217, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 1d20h, last write 1d20h
  Hold time is 90, keepalive interval is 30 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is inactive
  Keepalive timer is inactive
  Connect timer is active, time left: 00:00:17
  Connection interval is 20 seconds
  Failed connection attempts is 437
  Idle-restart timer is inactive
  BGP state is Connect
  Number of transitions to established: 2
  Last state was Active
  Last event was ConnectRetry
  Last sent notification:Hold Timer Expired Error/None, Last time 1d20h
  Last sent socket-error:Connect (Network is unreachable), Last time 02:46:22, First time 1d20h, Repeats 489
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

BGP neighbor is 10.0.0.221, remote AS 64512, internal link
 Description: Ribbon-221
  BGP version 4, remote router ID 10.0.0.221, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 1d01h, last write 1d01h
  Hold time is 180, keepalive interval is 60 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is inactive
  Keepalive timer is inactive
  Connect timer is active, time left: 00:00:58
  Connection interval is 148 seconds
  Failed connection attempts is 47
  Idle-restart timer is inactive
  BGP state is Active
  Number of transitions to established: 16
  Last state was Connect
  Last event was TransportError
  Last sent notification:Hold Timer Expired Error/None, Last time 1d01h, First time 5d01h, Repeats 6
  Last sent socket-error:Connect (Network is unreachable), Last time 00:02:13, First time 4d18h, Repeats 222
  Last rcvd socket-error:Connection reset by peer, Last time 1d20h, First time 5d18h, Repeats 8
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
    Opens:                 17        16
    Notifications:          7         0
    Updates:              956        51
    Keepalives:          6501     15241
    Route Refresh:         20        10
    Total messages:      7501     15318
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

BGP neighbor is 10.0.1.156, remote AS 64512, internal link
 Description: 2-23-5G-JUNIPER-156
  BGP version 4, remote router ID 10.0.0.156, VRF default
  Inherits configuration from and member of peer-group 2-23-5G-RR
  Last read 00:00:23, last write 00:00:04
  Hold time is 90, keepalive interval is 30 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:01:07
  Keepalive timer is active, time left: 00:00:19
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 1d19h
  Number of transitions to established: 3
  Last state was OpenConfirm
  Last event was RecvUpdate
  Last sent notification:Cease/other configuration change, Last time 1d20h
  Last rcvd notification:Cease/peer de-configured, Last time 1d19h
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
      Received 1d19h
      Number of stale paths removed after graceful restart: 0
      Number of paths received before End-of-RIB: 4
    L2VPN EVPN End-of-RIB received: Yes
      Received 1d19h
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
    Updates:               37       411
    Keepalives:          6228      5698
    Route Refresh:          0         0
    Total messages:      6269      6113
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    VPN-IPv4:                         2        14             14                   0
    IPv6 Unicast:                     0         0              0                   0
    EVPN:                             3        32             32                   0
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
    Round-trip Time (rtt/rtvar): 1.7ms/1.0ms
    Delayed Ack Timeout (ato): 40.0ms
    Congestion Window (cwnd): 3
    Slow-start Threshold (ssthresh): 7
    TCP Throughput: 20.26 Mbps
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
10.0.0.53/32    IS-IS SR IPv4   10          65                  115            
10.0.0.54/32    IS-IS SR IPv4   29          65                  115            
10.0.0.66/32    IS-IS SR IPv4   13          65                  115            
10.0.0.72/32    IS-IS SR IPv4   14          65                  115            
10.0.0.84/32    IS-IS SR IPv4   8           65                  115            
10.0.0.120/32   IS-IS SR IPv4   17          65                  115            
10.0.0.128/32   IS-IS SR IPv4   18          65                  115            
10.0.0.157/32   IS-IS SR IPv4   30          65                  115            
10.0.0.195/32   IS-IS SR IPv4   31          65                  115            
10.0.0.214/32   IS-IS SR IPv4   21          65                  115            
10.0.0.216/32   IS-IS SR IPv4   25          65                  115            
10.0.0.217/32   IS-IS SR IPv4   16          65                  115            
10.0.1.156/32   IS-IS SR IPv4   24          65                  115            
10.0.1.179/32   IS-IS SR IPv4   23          65                  115            

   IGP Metric    Metric Type
---------------- -----------
   11            metric     
   21            metric     
   11            metric     
   31            metric     
   21            metric     
   21            metric     
   21            metric     
   31            metric     
   51            metric     
   11            metric     
   21            metric     
   31            metric     
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
>C    10.0.0.30/32 [0 pref/0 metric] updated 1d21h ago
         via Loopback0, directly connected
>C    10.0.30.30/32 [0 pref/0 metric] updated 1d21h ago
         via Loopback1000, directly connected
>C    20.30.66.0/24 [0 pref/0 metric] updated 4d17h ago
         via Ethernet31, directly connected
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
>P    0.0.0.0/8 [1 pref/0 metric] updated 5d20h ago
         via Null0, directly connected [NF]
>P    127.0.0.0/8 [1 pref/0 metric] updated 5d20h ago
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
>I    10.0.0.53/32 [115 pref/11 metric] updated 17:14:03 ago
         via 20.30.66.66, Ethernet31
>I    10.0.0.54/32 [115 pref/21 metric] updated 00:22:02 ago
         via 20.30.66.66, Ethernet31
>I    10.0.0.66/32 [115 pref/11 metric] updated 1d20h ago
         via 20.30.66.66, Ethernet31
>I    10.0.0.72/32 [115 pref/31 metric] updated 17:14:03 ago
         via 20.30.66.66, Ethernet31
>I    10.0.0.84/32 [115 pref/21 metric] updated 1d20h ago
         via 20.30.66.66, Ethernet31
>I    10.0.0.120/32 [115 pref/21 metric] updated 17:14:03 ago
         via 20.30.66.66, Ethernet31
>I    10.0.0.128/32 [115 pref/21 metric] updated 17:14:03 ago
         via 20.30.66.66, Ethernet31
>I    10.0.0.157/32 [115 pref/31 metric] updated 02:46:29 ago
         via 20.30.66.66, Ethernet31
>I    10.0.0.195/32 [115 pref/51 metric] updated 01:29:53 ago
         via 20.30.66.66, Ethernet31
>I    10.0.0.214/32 [115 pref/11 metric] updated 18:10:36 ago
         via 20.30.66.66, Ethernet31
>I    10.0.0.216/32 [115 pref/21 metric] updated 1d01h ago
         via 20.30.66.66, Ethernet31
>I    10.0.0.217/32 [115 pref/31 metric] updated 00:57:44 ago
         via 20.30.66.66, Ethernet31
>I    10.0.1.156/32 [115 pref/11 metric] updated 01:26:20 ago
         via 20.30.66.66, Ethernet31
>I    10.0.1.179/32 [115 pref/11 metric] updated 1d20h ago
         via 20.30.66.66, Ethernet31
>I    20.53.66.0/24 [115 pref/11 metric] updated 17:14:05 ago
         via 20.30.66.66, Ethernet31
>I    20.53.72.0/24 [115 pref/21 metric] updated 17:14:03 ago
         via 20.30.66.66, Ethernet31
>I    20.53.120.0/24 [115 pref/21 metric] updated 17:14:03 ago
         via 20.30.66.66, Ethernet31
>I    20.53.128.0/24 [115 pref/21 metric] updated 17:14:03 ago
         via 20.30.66.66, Ethernet31
>I    20.53.185.0/24 [115 pref/21 metric] updated 17:14:03 ago
         via 20.30.66.66, Ethernet31
>I    20.53.216.0/24 [115 pref/21 metric] updated 17:14:03 ago
         via 20.30.66.66, Ethernet31
>I    20.54.66.0/24 [115 pref/11 metric] updated 00:22:04 ago
         via 20.30.66.66, Ethernet31
>I    20.66.84.0/24 [115 pref/11 metric] updated 1d20h ago
         via 20.30.66.66, Ethernet31
>I    20.66.156.0/24 [115 pref/11 metric] updated 01:26:41 ago
         via 20.30.66.66, Ethernet31
>I    20.66.179.0/24 [115 pref/11 metric] updated 1d20h ago
         via 20.30.66.66, Ethernet31
>I    20.66.214.0/24 [115 pref/11 metric] updated 18:10:47 ago
         via 20.30.66.66, Ethernet31
>I    20.120.217.0/24 [115 pref/21 metric] updated 17:14:03 ago
         via 20.30.66.66, Ethernet31
>I    20.128.157.0/24 [115 pref/31 metric] updated 02:46:51 ago
         via 20.30.66.66, Ethernet31
>I    20.128.217.0/24 [115 pref/31 metric] updated 00:58:22 ago
         via 20.30.66.66, Ethernet31
>I    20.156.216.0/24 [115 pref/31 metric] updated 01:14:23 ago
         via 20.30.66.66, Ethernet31
>I    20.157.195.0/24 [115 pref/41 metric] updated 01:30:14 ago
         via 20.30.66.66, Ethernet31
>I    20.157.217.0/24 [115 pref/41 metric] updated 02:46:29 ago
         via 20.30.66.66, Ethernet31
>I    50.20.120.0/24 [115 pref/21 metric] updated 17:14:03 ago
         via 20.30.66.66, Ethernet31
>I    192.168.20.0/23 [115 pref/21 metric] updated 17:14:03 ago
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
>C    2001:0:30:66::/64 [0 pref/0 metric] updated 4d17h ago
         via Ethernet31, directly connected
>C    2002::30/128 [0 pref/0 metric] updated 1d21h ago
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
>P    ::/96 [1 pref/0 metric] updated 5d20h ago
         via Null0, directly connected [NF]
>P    ::ffff:127.0.0.0/104 [1 pref/0 metric] updated 5d20h ago
         via :: [1 pref/1 metric] type ipv6
            via , directly connected
>P    fe80::/10 [1 pref/0 metric] updated 5d20h ago
```

## show platform sand l3 summary

```text
Number of vrfs: 5

Ipv4:
  Routes:       81  backlog:  0  unprogrammed:  0
  Adjacencies:  67  backlog:  0  unprogrammed:  0
Ipv6:
  Routes:       11  backlog:  0  unprogrammed:  0
  Adjacencies:  67  backlog:  0  unprogrammed:  0
Mpls:
  Routes:       15  backlog:  0  unprogrammed:  0
  Adjacencies:  1   backlog:  0  unprogrammed:  0

Jericho2 Ip Fecs:
  Non-ecmp fecs:  4129  ecmp fecs:  0  fec entries:  4129
Jericho2 Mpls Fecs:
  Non-ecmp fecs:  1  ecmp fecs:  0  fec entries:  1
Jericho2 Vxlan Tunnel Fecs:
  Non-ecmp fecs:  0  ecmp fecs:  0  fec entries:  0
  Number of vxlan tunnels configured: 0

Jericho2 Lpm Routes:
  Routes:   81  unprogrammed:   0   
  Routes6:  11  unprogrammed6:  0   
  Backlog:  0 

Jericho2 Lpm:
  TCAM entries used:   4   Percent free:  99  ADS2 entries used:   7  Percent free:  99
  Pivot buckets used:  6   Rows used:     2   Entries Per Bucket:  1  Percent free:  99
  Route buckets used:  17  Rows used:     3   Entries Per Bucket:  5  Percent free:  99

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
  FixedSystem: 14
Egress Sflow rewrite entries in use (in each fap):
  FixedSystem: 0

Egress rewrite chains in backlog: resource-full 0, no-interface 0

Glem entries used per fap :
  FixedSystem: 4112

Jericho2 Fec:
  Maximum FEC hierarchy levels:  2
  ReusedEcmp:  793  allocs:  5187  frees:  5156  shuffles:  0  cmds:  0
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
    Non-ecmp fecs:            32  ecmp fecs:            0  
    Non-ecmp (Percent free):  99  ecmp (Percent free):  100
  Level3  Fecs:
    Non-ecmp fecs:            30  ecmp fecs:            0  
    Non-ecmp (Percent free):  99  ecmp (Percent free):  100

Lpm Detail:
  Requests:  9766  cleanses:  1725  batches:  1725  avg batch size:  5

Jericho Arp:
  ArpTable writes:      131795  queued      0   
  IngressTable writes:  169111  queued      0   
  Coprocessors:         1       in CmdRing

Tunnel Counter Status
  Number of MPLS tunnels:                  14   
  Number of uncountable MPLS tunnels:      14   
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
|0  |10.0.0.53/32      |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318768|   -   
|0  |10.0.0.54/32      |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318768|   -   
|0  |10.0.0.66/32      |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318768|   -   
|0  |10.0.0.72/32      |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318768|   -   
|0  |10.0.0.84/32      |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318768|   -   
|0  |10.0.0.120/32     |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318768|   -   
|0  |10.0.0.128/32     |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318768|   -   
|0  |10.0.0.157/32     |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318768|   -   
|0  |10.0.0.195/32     |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318768|   -   
|0  |10.0.0.214/32     |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318768|   -   
|0  |10.0.0.216/32     |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318768|   -   
|0  |10.0.0.217/32     |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318768|   -   
|0  |10.0.1.156/32     |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318768|   -   
|0  |10.0.1.179/32     |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318768|   -   
|0  |10.0.30.30/32     |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.66.0/32     |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.66.30/32    |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.66.66/32    |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318992|   -   
|0  |20.30.66.255/32   |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.66.0/24     |TRAP | CoppSystemL3DstMiss|1020 |1020    | ArpTrap           |  -  |315691|   -   
|0  |20.53.66.0/24     |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318768|   -   
|0  |20.53.72.0/24     |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318768|   -   
|0  |20.53.120.0/24    |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318768|   -   
|0  |20.53.128.0/24    |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318768|   -   
|0  |20.53.185.0/24    |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318768|   -   
|0  |20.53.216.0/24    |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318768|   -   
|0  |20.54.66.0/24     |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318768|   -   
|0  |20.66.84.0/24     |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318768|   -   
|0  |20.66.156.0/24    |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318768|   -   
|0  |20.66.179.0/24    |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318768|   -   
|0  |20.66.214.0/24    |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318768|   -   
|0  |20.120.217.0/24   |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318768|   -   
|0  |20.128.157.0/24   |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318768|   -   
|0  |20.128.217.0/24   |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318768|   -   
|0  |20.156.216.0/24   |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318768|   -   
|0  |20.157.195.0/24   |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318768|   -   
|0  |20.157.217.0/24   |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318768|   -   
|0  |50.20.120.0/24    |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318768|   -   
|0  |127.0.0.0/8       |TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |  -  |314671|   -   
|0  |192.168.20.0/23   |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318768|   -   
|0  |0.0.0.0/0         |TRAP | CoppSystemL3LpmOver|0    |  -     | SlowReceive       |  -  |314669|   -   
|1  |0.0.0.0/8         |DROP | DROP               |0    |  -     |                   |  -  |318968|   -   
|1  |10.0.0.30/32      |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|1  |50.10.156.0/24    |ROUTE| FEC 318958         |0    |2097149 | 00:00:00:00:00:00 |  -  |183508|M 20456 16
|1  |50.10.179.0/24    |ROUTE| FEC 318958         |0    |2097118 | 00:00:00:00:00:00 |  -  |183548|M 20479 16
|1  |50.11.156.0/24    |ROUTE| FEC 318958         |0    |2097149 | 00:00:00:00:00:00 |  -  |183508|M 20456 16
|1  |127.0.0.0/8       |TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |  -  |314671|   -   
|1  |0.0.0.0/0         |TRAP | CoppSystemL3LpmOver|0    |  -     | SlowReceive       |  -  |314669|   -   
|2  |0.0.0.0/8         |DROP | DROP               |0    |  -     |                   |  -  |318970|   -   
|2  |10.128.0.30/32    |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|2  |50.128.156.0/24   |ROUTE| FEC 318958         |0    |2097148 | 00:00:00:00:00:00 |  -  |183512|M 20456 17
|2  |50.129.156.0/24   |ROUTE| FEC 318958         |0    |2097148 | 00:00:00:00:00:00 |  -  |183510|M 20456 17
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
|4  |50.10.54.0/24     |ROUTE| FEC 318958         |0    |2097151 | 00:00:00:00:00:00 |  -  |183502|M 20054 970000
|4  |50.10.72.0/24     |ROUTE| FEC 318958         |0    |2097138 | 00:00:00:00:00:00 |  -  |183516|M 20072 62000
|4  |50.10.84.0/24     |ROUTE| FEC 318958         |0    |2097133 | 00:00:00:00:00:00 |  -  |183506|M 20084 720897
|4  |50.10.120.0/24    |ROUTE| FEC 318958         |0    |2097150 | 00:00:00:00:00:00 |  -  |183504|M 20120 1407
|4  |50.10.128.0/24    |ROUTE| FEC 318958         |0    |2097140 | 00:00:00:00:00:00 |  -  |183536|M 20128 48063
|4  |50.10.179.0/24    |ROUTE| FEC 318958         |0    |2097117 | 00:00:00:00:00:00 |  -  |183550|M 20479 30
|4  |50.10.214.0/24    |ROUTE| FEC 318958         |0    |2097147 | 00:00:00:00:00:00 |  -  |183542|M 20214 500001
|4  |50.10.216.0/24    |ROUTE| FEC 318958         |0    |2097145 | 00:00:00:00:00:00 |  -  |183520|M 20216 1048575
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
|  -  |183502|ROUTE| FEC 318958         |   - |2097151 |                 - |Mpush 20054 970000
|  -  |183504|ROUTE| FEC 318958         |   - |2097150 |                 - |Mpush 20120 1407
|  -  |183506|ROUTE| FEC 318958         |   - |2097133 |                 - |Mpush 20084 720897
|  -  |183508|ROUTE| FEC 318958         |   - |2097149 |                 - |Mpush 20456 16
|  -  |183510|ROUTE| FEC 318958         |   - |2097148 |                 - |Mpush 20456 17
|  -  |183512|ROUTE| FEC 318958         |   - |2097148 |                 - |Mpush 20456 17
|  -  |183514|ROUTE| FEC 318958         |   - |2097148 |                 - |Mpush 20456 17
|  -  |183516|ROUTE| FEC 318958         |   - |2097138 |                 - |Mpush 20072 62000
|  -  |183520|ROUTE| FEC 318958         |   - |2097145 |                 - |Mpush 20216 1048575
|  -  |183536|ROUTE| FEC 318958         |   - |2097140 |                 - |Mpush 20128 48063
|  -  |183542|ROUTE| FEC 318958         |   - |2097147 |                 - |Mpush 20214 500001
|  -  |183548|ROUTE| FEC 318958         |   - |2097118 |                 - |Mpush 20479 16
|  -  |183550|ROUTE| FEC 318958         |   - |2097117 |                 - |Mpush 20479 30
|  -  |314666|TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |   -   
|  -  |314667|TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |   -   
|  -  |314669|TRAP | CoppSystemL3LpmOver|0    |  -     | SlowReceive       |   -   
|  -  |314671|TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |   -   
|  -  |315679|TRAP | CoppSystemL3DstMiss|1008 |1008    | ArpTrap           |   -   
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

## show interfaces counters queue | nz

```text
Aggregate VoQ Counters
Egress                     Traffic               Pkts             Octets           DropPkts         DropOctets
Port                       Class  
--------------------------------------------------------------------------------------------------------------
Et31                       TC1             4097013003       393313248288          822248698        78935875008
Et31                       TC6                3937143          377965728                  0                  0
Et31                       TC7                  37624            3563329                  0                  0
Et36                       TC7                     65              15535                  0                  0
Et39                       TC7                  28493            2243904                  0                  0
Et46/1                     TC1             4099397612       393542170720                  0                  0
Et46/1                     TC6                3937143          377965728                  0                  0
Et46/1                     TC7                     66              16841                  0                  0

Egress Queue Counters
Port                 Traffic DropPrec   DestType          OutEnqPkts      OutEnqOctets       OutDropPkts     OutDropOctets
                     Class
Et31                 TC1     DP0-3      UC                4097013015      393313249440                 0                 0
Et31                 TC6     DP0-3      UC                   3937558         378005568                 0                 0
Et31                 TC7     DP0-3      UC                     37622           2999406                 0                 0
Et36                 TC7     DP0-3      UC                        65             15080                 0                 0
Et39                 TC7     DP0-3      UC                     28661           1981329                 0                 0
Et46/1               TC1     DP0-3      UC                4098148881      393422292544                 0                 0
Et46/1               TC6     DP0-3      UC                   3937558         378005568                 0                 0
Et46/1               TC7     DP0-3      UC                        66             16379                 0                 0

```

## show sync-e esmc detail

```text
Interface Ethernet31
Last received quality level: QL-PRC, SSM: 0b0010/0xff, Type: Information
Last received source MAC: e46d.7fe3.c810
Last received valid message time: 2025-02-26 11:12:05
Last received extended QL TLV: not received
Last received invalid message time: never
Received valid message count: 74058
Received invalid message count: 0
ESMC messages received by type
Event: 4
Information: 74054
ESMC messages received by QL (SSM code)
QL-PRC (0b0010): 10204
QL-SSU-B (0b1000): 63854
Last sent quality level: QL-DNU, SSM: 0b1111/0xff, Type: Information
Last sent source MAC: c4ca.2b45.a234
Last sent message time: 2025-02-26 11:12:04
Sent message count: 74034
ESMC messages sent by type
Event: 1
Information: 74033
ESMC messages sent by QL (SSM code)
QL-EEC1 (0b1011): 23
QL-DNU (0b1111): 74011

Interface Ethernet39
Last received quality level: QL-DNU, SSM: 0b1111/0xff, Type: Information
Last received source MAC: 0011.0100.0001
Last received valid message time: 2025-02-26 11:12:05
Last received extended QL TLV: not received
Last received invalid message time: never
Received valid message count: 498
Received invalid message count: 0
ESMC messages received by type
Information: 498
ESMC messages received by QL (SSM code)
QL-DNU (0b1111): 498
Last sent quality level: QL-PRC, SSM: 0b0010/0xff, Type: Information
Last sent source MAC: c4ca.2b45.a23c
Last sent message time: 2025-02-26 11:12:05
Sent message count: 2269
ESMC messages sent by type
Information: 2269
ESMC messages sent by QL (SSM code)
QL-PRC (0b0010): 2269

```

## show sync-e selection

```text
Input      QL     Priority Status  
---------- ------ -------- --------
Ethernet31 QL-PRC      127 active  
Ethernet39 QL-DNU      127 unusable

```

## show ptp

```text
PTP Mode: Boundary Clock
PTP Profile: G8275.1
Clock Identity: c4:ca:2b:ff:ff:45:a2:15
Grandmaster Clock Identity: 00:b0:ae:ff:fe:0a:5b:70
Number of slave ports: 1
Number of master ports: 1
Slave port: Ethernet31
Offset From Master (nanoseconds): 1
Mean Path Delay (nanoseconds): 18
Steps Removed: 3
Skew (estimated local-to-master clock frequency ratio): 1.0
Last Sync Time: 11:12:05 UTC Feb 26 2025
Current PTP System Time: 11:12:05 UTC Feb 26 2025
   Interface       State        Transport    Delay    
                                             Mechanism
--------------- ------------ --------------- ---------
   Et31            Slave        layer2       e2e      
   Et39            Master       layer2       e2e      

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
Port state: Slave 
Sync interval: 0.0625 seconds
Announce interval: 0.125 seconds
Announce interval timeout multiplier: 3
Delay mechanism: end to end
Delay request message interval: 0.0625 seconds
Local Priority: 128
Transport mode: layer 2
Destination MAC address: 01:80:c2:00:00:0e
Announce messages sent: 0
Announce messages received: 587714
Sync messages sent: 0
Sync messages received: 1166087
Follow up messages sent: 0
Follow up messages received: 0
Delay request messages sent: 1160276
Delay request messages received: 0
Delay response messages sent: 0
Delay response messages received: 1160276
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
Port state: Master 
Sync interval: 0.0625 seconds
Announce interval: 0.125 seconds
Announce interval timeout multiplier: 3
Delay mechanism: end to end
Delay request message interval: 0.0625 seconds
Local Priority: 128
Transport mode: layer 2
Destination MAC address: 01:80:c2:00:00:0e
Announce messages sent: 3807
Announce messages received: 0
Sync messages sent: 7551
Sync messages received: 0
Follow up messages sent: 7551
Follow up messages received: 0
Delay request messages sent: 0
Delay request messages received: 7641
Delay response messages sent: 7641
Delay response messages received: 0
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
Announce messages sent: 0
Announce messages received: 587715
Sync messages sent: 0
Sync messages received: 1166088
Follow up messages sent: 0
Follow up messages received: 0
Delay request messages sent: 1160277
Delay request messages received: 0
Delay response messages sent: 0
Delay response messages received: 1160277
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
Interface Ethernet39
Announce messages sent: 3808
Announce messages received: 0
Sync messages sent: 7552
Sync messages received: 0
Follow up messages sent: 7552
Follow up messages received: 0
Delay request messages sent: 0
Delay request messages received: 7643
Delay response messages sent: 7643
Delay response messages received: 0
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

