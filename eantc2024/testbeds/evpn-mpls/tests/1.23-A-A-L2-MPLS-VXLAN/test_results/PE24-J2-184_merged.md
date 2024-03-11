# Test results for PE24-J2-184

## show version

```text
Arista DCS-7280SR3-40YC6-F
Hardware version: 11.02
Serial number: SGD231508WS
Hardware MAC address: c4ca.2b45.e739
System MAC address: c4ca.2b45.e739

Software image version: 4.32.0F-35483270.hudsonrel (engineering build)
Architecture: x86_64
Internal build version: 4.32.0F-35483270.hudsonrel
Internal build ID: bc4c8e97-b142-4c39-a634-2b265e10ac86
Image format version: 3.0
Image optimization: Default

Uptime: 20 hours and 40 minutes
Total memory: 8099732 kB
Free memory: 5117764 kB

```

## show interfaces status

```text
Port       Name   Status       Vlan     Duplex Speed  Type         Flags Encapsulation
Et1               connected    routed   full   10G    10GBASE-SRL                    
Et2               notconnect   1        full   25G    Not Present                    
Et3               notconnect   1        full   25G    Not Present                    
Et4               notconnect   1        full   25G    Not Present                    
Et5               connected    in Po200 full   10G    10GBASE-SRL                    
Et6               notconnect   1        full   25G    Not Present                    
Et7               notconnect   1        full   25G    Not Present                    
Et8               notconnect   1        full   25G    Not Present                    
Et9               notconnect   1        full   25G    Not Present                    
Et10              notconnect   1        full   25G    Not Present                    
Et11              notconnect   1        full   25G    Not Present                    
Et12              notconnect   1        full   25G    Not Present                    
Et13              notconnect   1        full   25G    Not Present                    
Et14              notconnect   1        full   25G    Not Present                    
Et15              notconnect   1        full   25G    Not Present                    
Et16              notconnect   1        full   25G    Not Present                    
Et17              notconnect   1        full   25G    Not Present                    
Et18              notconnect   1        full   25G    Not Present                    
Et19              notconnect   1        full   25G    Not Present                    
Et20              notconnect   1        full   25G    Not Present                    
Et21              notconnect   1        full   25G    Not Present                    
Et22              notconnect   1        full   25G    Not Present                    
Et23              notconnect   1        full   25G    Not Present                    
Et24              notconnect   1        full   25G    Not Present                    
Et25              notconnect   1        full   25G    Not Present                    
Et26              notconnect   1        full   25G    Not Present                    
Et27              notconnect   1        full   25G    Not Present                    
Et28              notconnect   1        full   25G    Not Present                    
Et29              notconnect   1        full   25G    Not Present                    
Et30              notconnect   1        full   25G    Not Present                    
Et31              notconnect   1        full   25G    Not Present                    
Et32              notconnect   1        full   25G    Not Present                    
Et33              notconnect   1        full   25G    Not Present                    
Et34              notconnect   1        full   25G    Not Present                    
Et35              notconnect   1        full   25G    Not Present                    
Et36              notconnect   1        full   25G    Not Present                    
Et37              notconnect   1        full   25G    Not Present                    
Et38              notconnect   1        full   25G    Not Present                    
Et39              errdisabled  1        full   10G    10GBASE-SRL                    
Et40              errdisabled  1        full   10G    10GBASE-SRL                    
Et41/1            notconnect   1        full   100G   Not Present                    
Et42/1            notconnect   1        full   100G   Not Present                    
Et43/1            notconnect   1        full   100G   Not Present                    
Et44/1            notconnect   1        full   100G   Not Present                    
Et45/1            notconnect   1        full   100G   Not Present                    
Et46/1            notconnect   1        full   100G   Not Present                    
Ma1               connected    routed   a-full a-1G   10/100/1000                    
Po200             connected    trunk    full   10G    N/A                            

```

## show bgp evpn summary

```text
BGP summary information for VRF default
Router identifier 100.0.0.184, local AS number 64512
Neighbor Status Codes: m - Under maintenance
  Neighbor    V AS           MsgRcvd   MsgSent  InQ OutQ  Up/Down State   PfxRcd PfxAcc
  100.0.0.183 4 64512            240       252    0    0 00:01:06 Estab   11     11
  100.0.3.41  4 64512            145       173    0    0 01:25:28 Estab   7      7
```

## show bgp evpn instance

```text
EVPN instance: VLAN 2068
  Route distinguisher: 100.0.0.184:2068
  Route target import: Route-Target-AS:2068:2068
  Route target export: Route-Target-AS:2068:2068
  Service interface: VLAN-based
  Local MPLS IP address: 100.0.0.184
  VXLAN: disabled
  MPLS: enabled
  Label allocation mode: per-instance
EVPN instance: VLAN 2301
  Route distinguisher: 100.0.0.184:2301
  Route target import: Route-Target-AS:2301:2301
  Route target export: Route-Target-AS:2301:2301
  Service interface: VLAN-based
  Local MPLS IP address: 100.0.0.184
  VXLAN: disabled
  MPLS: enabled
  Label allocation mode: per-instance
EVPN instance: VLAN 2302
  Route distinguisher: 100.0.0.184:2302
  Route target import: Route-Target-AS:2302:2302
  Route target export: Route-Target-AS:2302:2302
  Service interface: VLAN-based
  Local MPLS IP address: 100.0.0.184
  VXLAN: disabled
  MPLS: enabled
  Label allocation mode: per-instance
EVPN instance: VLAN 3301
  Route distinguisher: 100.0.0.184:3301
  Route target import: Route-Target-AS:3301:65414
  Route target export: Route-Target-AS:3301:65414
  Service interface: VLAN-based
  Local MPLS IP address: 100.0.0.184
  VXLAN: disabled
  MPLS: enabled
  Label allocation mode: per-instance
  MAC route MPLS label: 1047712
  IMET route MPLS label: 1048348
  AD route MPLS label: 1047712
  Remote ethernet segment:
    ESI: 0000:00d1:0000:0000:00d1
    Active TEPs: 100.0.3.41
    ESI: 0011:1111:1111:1111:1111
    Active TEPs: 100.0.0.183
  Local ethernet segment:
    ESI: 0000:0000:0000:0183:0184
      Interface: Port-Channel200
      Mode: all-active
      State: up
      ESI label: 1045148
      ES-Import RT: 00:00:18:30:01:84
      DF election algorithm: preference
      Designated forwarder: 100.0.0.184
EVPN instance: VLAN 3302
  Route distinguisher: 100.0.0.184:3302
  Route target import: Route-Target-AS:3302:65414
  Route target export: Route-Target-AS:3302:65414
  Service interface: VLAN-based
  Local MPLS IP address: 100.0.0.184
  VXLAN: disabled
  MPLS: enabled
  Label allocation mode: per-instance
  MAC route MPLS label: 1036415
  IMET route MPLS label: 1043923
  AD route MPLS label: 1036415
  Remote ethernet segment:
    ESI: 0000:00d1:0000:0000:00d1
    Active TEPs: 100.0.3.41
    ESI: 0011:1111:1111:1111:1111
    Active TEPs: 100.0.0.183
  Local ethernet segment:
    ESI: 0000:0000:0000:0183:0184
      Interface: Port-Channel200
      Mode: all-active
      State: up
      ESI label: 1045148
      ES-Import RT: 00:00:18:30:01:84
      DF election algorithm: preference
      Designated forwarder: 100.0.0.184
EVPN instance: VLAN-aware bundle 2303-2304
  Route distinguisher: 100.0.0.184:2303
  Route target import: Route-Target-AS:2303:2303
  Route target export: Route-Target-AS:2303:2303
  Service interface: VLAN-aware bundle
  Local MPLS IP address: 100.0.0.184
  VXLAN: disabled
  MPLS: enabled
  Label allocation mode: per-instance
```

## show ip route vrf tenant-a

```text

VRF: tenant-a
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


```

## show interfaces counters rates | nz

```text
Port      Name      Intvl  In Mbps      %  In Kpps Out Mbps      % Out Kpps
Et1                  0:05    198.8   2.0%       24    199.6   2.0%       24
Et5                  0:05    195.3   2.0%       24    195.3   2.0%       24
Ma1                  0:05      0.0   0.0%        0      0.1   0.0%        0
Po200                0:05    195.3   2.0%       24    195.3   2.0%       24
```

## show running-config section router bgp

```text
router bgp 64512
   router-id 100.0.0.184
   distance bgp 20 200 200
   maximum-paths 8 ecmp 16
   bgp bestpath skip next-hop igp-cost
   neighbor RR_EVPN peer group
   neighbor RR_EVPN remote-as 64512
   neighbor RR_EVPN next-hop-unchanged
   neighbor RR_EVPN update-source Loopback0
   neighbor RR_EVPN send-community
   neighbor RR_EVPN maximum-routes 12000
   neighbor 100.0.0.183 peer group RR_EVPN
   neighbor 100.0.3.41 peer group RR_EVPN
   redistribute connected
   !
   vlan 2068
      rd 100.0.0.184:2068
      route-target both 2068:2068
      redistribute learned
      redistribute static
   !
   vlan 2301
      rd 100.0.0.184:2301
      route-target both 2301:2301
      redistribute learned
      redistribute static
   !
   vlan 2302
      rd 100.0.0.184:2302
      route-target both 2302:2302
      redistribute learned
      redistribute static
   !
   vlan 3301
      rd 100.0.0.184:3301
      route-target both 3301:65414
      redistribute learned
      redistribute static
   !
   vlan 3302
      rd 100.0.0.184:3302
      route-target both 3302:65414
      redistribute learned
      redistribute static
   !
   vlan-aware-bundle 2303-2304
      rd 100.0.0.184:2303
      route-target both 2303:2303
      redistribute learned
      redistribute static
      vlan 2303-2304
   !
   address-family evpn
      bgp additional-paths receive
      neighbor RR_EVPN activate
      neighbor RR_EVPN encapsulation mpls next-hop-self source-interface Loopback0
   !
   address-family ipv4
      no neighbor RR_EVPN activate
   !
   vrf L2GW
      rd 100.0.0.184:1023
      route-target import evpn 1023:1023
      route-target export evpn 1023:1023
   !
   vrf tenant-a
      rd 100.0.0.184:2000
      route-target import evpn 1000:1000
      route-target export evpn 1000:1000
      maximum-paths 4 ecmp 4
      no bgp additional-paths receive
      redistribute connected
```

## show running-config section interfaces

```text
```

## show bgp evpn mac

```text
VLAN  Label  Encap MAC                Tunnel Endpoint    Seq#
----- ------ ----- ------------------ ------------------ ----
0     103629 MPLS  0000.0181.0181     100.0.0.183        Stic
      2                                                  ky  
0     24000  MPLS  0000.0181.0181     100.0.3.41         Stic
                                                         ky  
0     103629 MPLS  0018.6380.ef6a     100.0.0.183        -   
      2                                                      
0     24000  MPLS  0018.6380.ef6a     100.0.3.41         -   
0     104771 MPLS  b0aa.fb45.eeee     Local              -   
      2                                                      
0     104771 MPLS  0018.6380.ef68     Local              -   
      2                                                      
0     103629 MPLS  b0aa.fb45.ebeb     100.0.0.183        -   
      2                                                      
0     24000  MPLS  b0aa.fb45.ebeb     100.0.3.41         -   
0     104771 MPLS  0000.0184.0184     Local              Stic
      2                                                  ky  
```

## show platform fap mac-address-table vlan 3301

```text
Fap0: Mac Table Poller
Hardware Mac Table Polling Interval (sec) : 2.00
 --------------------------------------------------------------------------------
|                                    MAC Table                                   |
|--------------------------------------------------------------------------------|
|     |                   |     Destination      |    Aging  | SA |     Intf     |
| FID |         MAC       |    Type    |    Val  |Stt|Dyn|Prg| Drp|     Name     |
|--------------------------------------------------------------------------------|
| 3301| b0:aa:fb:45:ee:ee |         LAG| 0x00000 | 0 | Y | N | N  |         Po200|
| 3301| 00:18:63:80:ef:68 |         LAG| 0x00000 | 0 | Y | N | N  |         Po200|
| 3301| 00:18:63:80:ef:6a |         FEC| 0x20000 | 0 | Y | Y | N  |    MplsTrunk1|
| 3301| b0:aa:fb:45:eb:eb |         FEC| 0x20000 | 0 | Y | Y | N  |    MplsTrunk1|
| 3301| 00:00:01:81:01:81 |         FEC| 0x20000 | 0 | N | Y | N  |    MplsTrunk1|
| 3301| 00:00:01:84:01:84 |         LAG| 0x00000 | 0 | N | Y | N  |         Po200|
 --------------------------------------------------------------------------------
```

## show platform fap fec all

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
|  -  |131072|ROUTE| FEC 183510         |   - |2097150 |                 - |Mpush 900183 1036292
|  -  |183502|DROP | DROP               |0    |  -     |                   |   -   
|  -  |183503|DROP | DROP               |0    |  -     |                   |   -   
|  -  |183504|DROP | DROP               |0    |  -     |                   |   -   
|  -  |183505|DROP | DROP               |0    |  -     |                   |   -   
|  -  |183506|ROUTE| Et1                |1006 |103421  | 44:4c:a8:73:9c:0d |   -   
|  -  |183507|ROUTE| Et1                |1006 |103421  | 44:4c:a8:73:9c:0d |   -   
|  -  |183508|ROUTE| Et1                |1006 |103421  | 44:4c:a8:73:9c:0d |   -   
|  -  |183510|ROUTE| Et1                |1006 |103421  | 44:4c:a8:73:9c:0d |   -   
|  -  |314667|TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |   -   
|  -  |314670|TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |   -   
|  -  |314671|TRAP | CoppSystemL3LpmOver|0    |  -     | SlowReceive       |   -   
|  -  |314672|TRAP | CoppSystemL3LpmOver|0    |  -     | SlowReceive       |   -   
|  -  |314673|TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |   -   
|  -  |315679|TRAP | CoppSystemL3DstMiss|1006 |1006    | ArpTrap           |   -   

```

