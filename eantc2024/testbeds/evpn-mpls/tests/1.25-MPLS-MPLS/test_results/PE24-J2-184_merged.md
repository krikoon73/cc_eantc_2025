# Test results for PE24-J2-184

## show version

```text
Arista DCS-7280SR3-40YC6-F
Hardware version: 11.02
Serial number: SGD231508WS
Hardware MAC address: c4ca.2b45.e739
System MAC address: c4ca.2b45.e739

Software image version: 4.28.6.1M
Architecture: i686
Internal build version: 4.28.6.1M-30820457.42861M
Internal build ID: 6064e036-b8b7-433c-8425-5e378eaa9915
Image format version: 3.0
Image optimization: Default

Uptime: 1 day, 6 hours and 35 minutes
Total memory: 8147100 kB
Free memory: 5743628 kB

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
Router identifier 100.0.0.184, local AS number 65184
Neighbor Status Codes: m - Under maintenance
  Neighbor    V AS           MsgRcvd   MsgSent  InQ OutQ  Up/Down State   PfxRcd PfxAcc
  100.0.0.180 4 64513           1936      1691    0    0 01:05:08 Estab   25     25
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
  MAC route MPLS label: 1044425
  IMET route MPLS label: 1036411
  AD route MPLS label: 1044425
  Local ethernet segment:
    ESI: 0000:0000:0000:0183:0184
      Interface: Port-Channel200
      Mode: all-active
      State: up
      ESI label: 1039535
      ES-Import RT: 00:00:18:30:01:84
      Designated forwarder: 100.0.0.184
EVPN instance: VLAN 2301
  Route distinguisher: 100.0.0.184:2301
  Route target import: Route-Target-AS:2301:2301
  Route target export: Route-Target-AS:2301:2301
  Service interface: VLAN-based
  Local MPLS IP address: 100.0.0.184
  VXLAN: disabled
  MPLS: enabled
  Label allocation mode: per-instance
  MAC route MPLS label: 1044674
  IMET route MPLS label: 1048063
  AD route MPLS label: 1044674
  Local ethernet segment:
    ESI: 0000:0000:0000:0183:0184
      Interface: Port-Channel200
      Mode: all-active
      State: up
      ESI label: 1039535
      ES-Import RT: 00:00:18:30:01:84
      Designated forwarder: 100.0.0.184
EVPN instance: VLAN 2302
  Route distinguisher: 100.0.0.184:2302
  Route target import: Route-Target-AS:2302:2302
  Route target export: Route-Target-AS:2302:2302
  Service interface: VLAN-based
  Local MPLS IP address: 100.0.0.184
  VXLAN: disabled
  MPLS: enabled
  Label allocation mode: per-instance
  MAC route MPLS label: 1045917
  IMET route MPLS label: 1043097
  AD route MPLS label: 1045917
  Local ethernet segment:
    ESI: 0000:0000:0000:0183:0184
      Interface: Port-Channel200
      Mode: all-active
      State: up
      ESI label: 1039535
      ES-Import RT: 00:00:18:30:01:84
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
  MAC route MPLS label: 1042255
  IMET route MPLS label: 1045658
  AD route MPLS label: 1042255
  Local ethernet segment:
    ESI: 0000:0000:0000:0183:0184
      Interface: Port-Channel200
      Mode: all-active
      State: up
      ESI label: 1039535
      ES-Import RT: 00:00:18:30:01:84
      Designated forwarder: 100.0.0.184
```

## show ip route vrf tenant-a

```text

VRF: tenant-a
Codes: C - connected, S - static, K - kernel, 
       O - OSPF, IA - OSPF inter area, E1 - OSPF external type 1,
       E2 - OSPF external type 2, N1 - OSPF NSSA external type 1,
       N2 - OSPF NSSA external type2, B - Other BGP Routes,
       B I - iBGP, B E - eBGP, R - RIP, I L1 - IS-IS level 1,
       I L2 - IS-IS level 2, O3 - OSPFv3, A B - BGP Aggregate,
       A O - OSPF Summary, NG - Nexthop Group Static Route,
       V - VXLAN Control Service, M - Martian,
       DH - DHCP client installed default route,
       DP - Dynamic Policy Route, L - VRF Leaked,
       G  - gRIBI, RC - Route Cache Route

Gateway of last resort is not set

 B E      20.10.18.0/24 [20/0] via 100.0.0.183/32, IS-IS SR tunnel index 6, label 116385
                                  via 20.180.184.180, Ethernet1, label 900183
                               via 100.0.37.9/32, IS-IS SR tunnel index 8, label 16
                                  via 20.180.184.180, Ethernet1, label 900379
                               via 100.0.3.41/32, IS-IS SR tunnel index 13, label 24006
                                  via 20.180.184.180, Ethernet1, label 900341
                               via 100.0.0.34/32, IS-IS SR tunnel index 18, label 48121
                                  via 20.180.184.180, Ethernet1, label 900034
 B E      20.10.21.0/24 [20/0] via 100.0.0.183/32, IS-IS SR tunnel index 6, label 116385
                                  via 20.180.184.180, Ethernet1, label 900183
                               via 100.0.37.9/32, IS-IS SR tunnel index 8, label 16
                                  via 20.180.184.180, Ethernet1, label 900379
                               via 100.0.3.41/32, IS-IS SR tunnel index 13, label 24006
                                  via 20.180.184.180, Ethernet1, label 900341
                               via 100.0.0.34/32, IS-IS SR tunnel index 18, label 48121
                                  via 20.180.184.180, Ethernet1, label 900034
 B E      20.10.31.0/24 [20/0] via 100.0.0.183/32, IS-IS SR tunnel index 6, label 116385
                                  via 20.180.184.180, Ethernet1, label 900183
                               via 100.0.37.9/32, IS-IS SR tunnel index 8, label 16
                                  via 20.180.184.180, Ethernet1, label 900379
                               via 100.0.3.41/32, IS-IS SR tunnel index 13, label 24006
                                  via 20.180.184.180, Ethernet1, label 900341
                               via 100.0.0.34/32, IS-IS SR tunnel index 18, label 48121
                                  via 20.180.184.180, Ethernet1, label 900034
 C        20.10.68.0/24 is directly connected, Vlan2068
 B E      20.10.108.0/24 [20/0] via 100.0.0.183/32, IS-IS SR tunnel index 6, label 116385
                                   via 20.180.184.180, Ethernet1, label 900183
                                via 100.0.37.9/32, IS-IS SR tunnel index 8, label 16
                                   via 20.180.184.180, Ethernet1, label 900379
                                via 100.0.3.41/32, IS-IS SR tunnel index 13, label 24006
                                   via 20.180.184.180, Ethernet1, label 900341
                                via 100.0.0.34/32, IS-IS SR tunnel index 18, label 48121
                                   via 20.180.184.180, Ethernet1, label 900034

```

## show interfaces counters rates | nz

```text
Port      Name        Intvl   In Mbps      %  In Kpps  Out Mbps      % Out Kpps
Et1                    0:05       2.7   0.0%        0       2.7   0.0%        0
Et5                    0:05       2.7   0.0%        0       2.7   0.0%        0
Po200                  0:05       2.7   0.0%        0       2.7   0.0%        0
```

## show running-config section router bgp

```text
router bgp 65184
   router-id 100.0.0.184
   distance bgp 20 200 200
   maximum-paths 8 ecmp 16
   bgp bestpath skip next-hop igp-cost
   neighbor RR_EVPN peer group
   neighbor RR_EVPN remote-as 64513
   neighbor RR_EVPN next-hop-unchanged
   neighbor RR_EVPN update-source Loopback0
   neighbor RR_EVPN ebgp-multihop 10
   neighbor RR_EVPN send-community
   neighbor RR_EVPN maximum-routes 12000
   neighbor 100.0.0.180 peer group RR_EVPN
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

## show bgp vpn-ipv4 detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.184, local AS number 65184
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

