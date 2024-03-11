# Test results for PE23-J2-183

## show version

```text
Arista DCS-7280SR3-40YC6-F
Hardware version: 11.00
Serial number: SGD22310589
Hardware MAC address: c4ca.2b45.ef6d
System MAC address: c4ca.2b45.ef6d

Software image version: 4.32.0F-35483270.hudsonrel (engineering build)
Architecture: x86_64
Internal build version: 4.32.0F-35483270.hudsonrel
Internal build ID: bc4c8e97-b142-4c39-a634-2b265e10ac86
Image format version: 3.0
Image optimization: Default

Uptime: 18 hours and 32 minutes
Total memory: 8099732 kB
Free memory: 5081964 kB

```

## show interfaces status

```text
Port       Name   Status       Vlan     Duplex Speed  Type         Flags Encapsulation
Et1               connected    routed   full   10G    10GBASE-SRL                    
Et2               notconnect   1        full   25G    Not Present                    
Et3               notconnect   1        full   25G    Not Present                    
Et4               notconnect   1        full   25G    Not Present                    
Et5               errdisabled  in Po200 full   10G    10GBASE-SRL                    
Et6               notconnect   1        full   10G    10GBASE-LR                     
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
Et39              notconnect   1        full   25G    Not Present                    
Et40              notconnect   1        full   25G    Not Present                    
Et41/1            notconnect   1        full   100G   Not Present                    
Et42/1            notconnect   1        full   100G   Not Present                    
Et43/1            notconnect   1        full   100G   Not Present                    
Et44/1            notconnect   1        full   100G   Not Present                    
Et45/1            notconnect   1        full   100G   Not Present                    
Et46/1            notconnect   1        full   100G   Not Present                    
Ma1               connected    routed   a-full a-1G   10/100/1000                    
Po200             disabled     trunk    full   unconf N/A                            

```

## show bgp evpn summary

```text
BGP summary information for VRF default
Router identifier 100.0.0.183, local AS number 64512
Neighbor Status Codes: m - Under maintenance
  Description              Neighbor    V AS           MsgRcvd   MsgSent  InQ OutQ  Up/Down State   PfxRcd PfxAcc
  RR_EVPN-VXLAN            100.0.0.180 4 64512           1770      1359    0    0 00:01:10 Estab   265    262
                           100.0.0.184 4 64512            259       278    0    0 00:01:06 Estab   9      9
                           100.0.3.41  4 64512           1242      1471    0    0 00:01:06 Estab   11     8
```

## show bgp evpn instance

```text
EVPN instance: VLAN 3301
  Route distinguisher: 100.0.0.183:3301
  Route distinguisher remote: 100.0.0.183:3301
  Route target import: Route-Target-AS:3301:65412
  Route target export: Route-Target-AS:3301:65412
  Route target import remote: Route-Target-AS:3301:65414
  Route target export remote: Route-Target-AS:3301:65414
  Service interface: VLAN-based
  Local VXLAN IP address: 100.0.0.183
  Local MPLS IP address: 100.0.0.183
  VXLAN: enabled
  MPLS: enabled
  Label allocation mode: per-instance
  MAC route MPLS label: 1036292
  IMET route MPLS label: 1036293
  AD route MPLS label: 1036292
  Local ethernet segment:
    ESI: 0011:1111:1111:1111:1111
      Interface: Vxlan1
      Mode: all-active
      State: up
      ESI label: 1036288
      ES-Import RT: 11:11:11:11:11:11
      DF election algorithm: modulus
      Designated forwarder: 100.0.0.183
    ESI: 0000:00d1:0000:0000:00d1
      Interface: MplsTrunk1
      Mode: all-active
      State: up
      ESI label: 1044071
      ES-Import RT: 00:00:d1:00:00:d1
      DF election algorithm: modulus
      Designated forwarder: 100.0.3.41
      Non-Designated forwarder: 100.0.0.183
EVPN instance: VLAN 3302
  Route distinguisher: 100.0.0.183:3302
  Route distinguisher remote: 100.0.0.183:3302
  Route target import: Route-Target-AS:3302:65412
  Route target export: Route-Target-AS:3302:65412
  Route target import remote: Route-Target-AS:3302:65414
  Route target export remote: Route-Target-AS:3302:65414
  Service interface: VLAN-based
  Local VXLAN IP address: 100.0.0.183
  Local MPLS IP address: 100.0.0.183
  VXLAN: enabled
  MPLS: enabled
  Label allocation mode: per-instance
  MAC route MPLS label: 1036290
  IMET route MPLS label: 1036291
  AD route MPLS label: 1036290
  Local ethernet segment:
    ESI: 0011:1111:1111:1111:1111
      Interface: Vxlan1
      Mode: all-active
      State: up
      ESI label: 1036288
      ES-Import RT: 11:11:11:11:11:11
      DF election algorithm: modulus
      Designated forwarder: 100.0.0.183
    ESI: 0000:00d1:0000:0000:00d1
      Interface: MplsTrunk1
      Mode: all-active
      State: up
      ESI label: 1044071
      ES-Import RT: 00:00:d1:00:00:d1
      DF election algorithm: modulus
      Designated forwarder: 100.0.0.183
      Non-Designated forwarder: 100.0.3.41
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
Et1                  5:00    104.3   1.1%       12     99.7   1.0%       11
```

## show running-config section router bgp

```text
router bgp 64512
   router-id 100.0.0.183
   distance bgp 20 200 200
   maximum-paths 4 ecmp 16
   bgp bestpath d-path
   neighbor RR_EVPN peer group
   neighbor RR_EVPN remote-as 64512
   neighbor RR_EVPN next-hop-unchanged
   neighbor RR_EVPN update-source Loopback0
   neighbor RR_EVPN send-community
   neighbor RR_EVPN maximum-routes 12000
   neighbor RR_EVPN-VXLAN peer group
   neighbor RR_EVPN-VXLAN remote-as 64512
   neighbor RR_EVPN-VXLAN next-hop-unchanged
   neighbor RR_EVPN-VXLAN update-source Loopback0
   neighbor RR_EVPN-VXLAN ebgp-multihop 3
   neighbor RR_EVPN-VXLAN send-community
   neighbor bgp peer group
   neighbor bgp rib-in pre-policy retain all
   neighbor 100.0.0.180 peer group RR_EVPN-VXLAN
   neighbor 100.0.0.180 description RR_EVPN-VXLAN
   neighbor 100.0.0.184 peer group RR_EVPN
   neighbor 100.0.3.41 peer group RR_EVPN
   redistribute connected
   !
   vlan 3301
      rd evpn domain all 100.0.0.183:3301
      route-target import export 3301:65412
      route-target import export evpn domain remote 3301:65414
      redistribute learned
      redistribute static
   !
   vlan 3302
      rd evpn domain all 100.0.0.183:3302
      route-target import export 3302:65412
      route-target import export evpn domain remote 3302:65414
      redistribute learned
      redistribute static
   !
   address-family evpn
      neighbor RR_EVPN activate
      neighbor RR_EVPN rcf in evpnDciMhBlockGwRx()
      neighbor RR_EVPN rcf out evpnDciMhBlockGwTxToMpls()
      neighbor RR_EVPN encapsulation mpls next-hop-self source-interface Loopback0
      neighbor RR_EVPN domain remote
      neighbor RR_EVPN-VXLAN activate
      neighbor RR_EVPN-VXLAN rcf in evpnDciMhBlockGwRx()
      neighbor RR_EVPN-VXLAN rcf out evpnDciMhBlockGwTxToEvpn()
      neighbor RR_EVPN-VXLAN encapsulation vxlan 
      layer-2 fec in-place update
      !
      evpn ethernet-segment domain local
         identifier 0011:1111:1111:1111:1111
         route-target import 11:11:11:11:11:11
      !
      evpn ethernet-segment domain remote
         identifier 0000:00d1:0000:0000:00d1
         designated-forwarder election algorithm preference 150
         route-target import 00:00:d1:00:00:d1
   !
   address-family ipv4
      no neighbor RR_EVPN activate
      no neighbor RR_EVPN-VXLAN activate
   !
   vrf L2GW
      rd 100.0.0.183:1023
      rd evpn domain remote 100.0.0.181:2000
      route-target import evpn 1023:1023
      route-target import evpn domain remote 1023:1023
      route-target export evpn 1023:1023
      route-target export evpn domain remote 1023:1023
   !
   vrf tenant-a
      rd 100.0.0.183:2000
      evpn multicast
      route-target import evpn 1000:1000
      route-target import vpn-ipv4 5000:5000
      route-target export evpn 1000:1000
      route-target export vpn-ipv4 5000:5000
      redistribute connected
```

## show running-config section interfaces

```text
```

## show bgp evpn mac

```text
VLAN  Label  Encap MAC                Tunnel Endpoint    Seq#
----- ------ ----- ------------------ ------------------ ----
0     104771 MPLS  0018.6380.ef68     100.0.0.184        -   
      2                                                      
0     104771 MPLS  0000.0184.0184     100.0.0.184        Stic
      2                                                  ky  
0     104771 MPLS  b0aa.fb45.eeee     100.0.0.184        -   
      2                                                      
3301  3301   VXLAN 0018.6380.ef6a     100.0.0.181        -   
3301  3301   VXLAN b0aa.fb45.ebeb     100.0.0.181        -   
3301  3301   VXLAN 0000.0181.0181     100.0.0.181        Stic
                                                         ky  
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
| 3301| b0:aa:fb:45:eb:eb |         FEC| 0x2ccd4 | 0 | Y | Y | N  |           Vx1|
| 3301| 00:18:63:80:ef:68 |         FEC| 0x20001 | 0 | Y | Y | N  |    MplsTrunk1|
| 3301| 00:18:63:80:ef:6a |         FEC| 0x2ccd4 | 0 | Y | Y | N  |           Vx1|
| 3301| 00:00:01:84:01:84 |         FEC| 0x20001 | 0 | N | Y | N  |    MplsTrunk1|
| 3301| b0:aa:fb:45:ee:ee |         FEC| 0x20001 | 0 | Y | Y | N  |    MplsTrunk1|
| 3301| 00:00:01:81:01:81 |         FEC| 0x2ccd4 | 0 | N | Y | N  |           Vx1|
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
|  -  |131072|ROUTE| FEC 183510         |4093 |103425  | 28:99:3a:8f:8f:6f |   -   
|  -  |131073|ROUTE| FEC 183511         |   - |2097151 |                 - |Mpush 900184 1047712
|  -  |183502|DROP | DROP               |0    |  -     |                   |   -   
|  -  |183503|ROUTE| Et1                |1006 |103421  | 44:4c:a8:73:9c:0d |   -   
|  -  |183504|DROP | DROP               |0    |  -     |                   |   -   
|  -  |183505|DROP | DROP               |0    |  -     |                   |   -   
|  -  |183506|ROUTE| Et1                |1006 |103421  | 44:4c:a8:73:9c:0d |   -   
|  -  |183507|ROUTE| Et1                |1006 |103421  | 44:4c:a8:73:9c:0d |   -   
|  -  |183509|DROP | DROP               |0    |  -     |                   |   -   
|  -  |183510|ROUTE| Et1                |1006 |103424  | 44:4c:a8:73:9c:0d |T 100.0.0.181
|  -  |183511|ROUTE| Et1                |1006 |103421  | 44:4c:a8:73:9c:0d |   -   
|  -  |314667|TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |   -   
|  -  |314670|TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |   -   
|  -  |314671|TRAP | CoppSystemL3LpmOver|0    |  -     | SlowReceive       |   -   
|  -  |314672|TRAP | CoppSystemL3LpmOver|0    |  -     | SlowReceive       |   -   
|  -  |314673|TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |   -   
|  -  |315679|TRAP | CoppSystemL3DstMiss|1006 |1006    | ArpTrap           |   -   

```

