# Test results for PE23-J2-183

## show version

```text
Arista DCS-7280SR3-40YC6-F
Hardware version: 11.00
Serial number: SGD22310589
Hardware MAC address: c4ca.2b45.ef6d
System MAC address: c4ca.2b45.ef6d

Software image version: 4.28.6.1M
Architecture: i686
Internal build version: 4.28.6.1M-30820457.42861M
Internal build ID: 6064e036-b8b7-433c-8425-5e378eaa9915
Image format version: 3.0
Image optimization: Default

Uptime: 1 day, 6 hours and 35 minutes
Total memory: 8147100 kB
Free memory: 5772420 kB

```

## show interfaces status

```text
Port       Name   Status       Vlan     Duplex Speed  Type         Flags Encapsulation
Et1               connected    routed   full   10G    10GBASE-SRL                    
Et2               notconnect   1        full   25G    Not Present                    
Et3               notconnect   1        full   25G    Not Present                    
Et4               notconnect   1        full   25G    Not Present                    
Et5               notconnect   in Po200 full   10G    10GBASE-SRL                    
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
Po200             notconnect   trunk    full   unconf N/A                            

```

## show bgp evpn summary

```text
BGP summary information for VRF default
Router identifier 100.0.0.183, local AS number 64512
Neighbor Status Codes: m - Under maintenance
  Description              Neighbor    V AS           MsgRcvd   MsgSent  InQ OutQ  Up/Down State   PfxRcd PfxAcc
  RR_ANET                  100.0.0.180 4 64513           2064      1648    0    0 00:37:14 Estab   12     12
```

## show bgp evpn instance

```text
EVPN instance: VLAN 2068
  Route distinguisher: 100.0.0.183:2068
  Route target import: Route-Target-AS:2068:2068
  Route target export: Route-Target-AS:2068:2068
  Service interface: VLAN-based
  Local MPLS IP address: 100.0.0.183
  VXLAN: disabled
  MPLS: enabled
  Label allocation mode: per-instance
  MAC route MPLS label: 1042979
  IMET route MPLS label: 1038234
  AD route MPLS label: 1042979
  Local ethernet segment:
    ESI: 0000:0000:0000:0183:0184
      Interface: Port-Channel200
      Mode: all-active
      State: down
      ESI label: 1039535
      ES-Import RT: 00:00:18:30:01:84
      DF election state: pending
      Designated forwarder: 
EVPN instance: VLAN 2301
  Route distinguisher: 100.0.0.183:2301
  Route target import: Route-Target-AS:2301:2301
  Route target export: Route-Target-AS:2301:2301
  Service interface: VLAN-based
  Local MPLS IP address: 100.0.0.183
  VXLAN: disabled
  MPLS: enabled
  Label allocation mode: per-instance
  MAC route MPLS label: 1036801
  IMET route MPLS label: 1039671
  AD route MPLS label: 1036801
  Local ethernet segment:
    ESI: 0000:0000:0000:0183:0184
      Interface: Port-Channel200
      Mode: all-active
      State: down
      ESI label: 1039535
      ES-Import RT: 00:00:18:30:01:84
      DF election state: pending
      Designated forwarder: 
EVPN instance: VLAN 2302
  Route distinguisher: 100.0.0.183:2302
  Route target import: Route-Target-AS:2302:2302
  Route target export: Route-Target-AS:2302:2302
  Service interface: VLAN-based
  Local MPLS IP address: 100.0.0.183
  VXLAN: disabled
  MPLS: enabled
  Label allocation mode: per-instance
  MAC route MPLS label: 1040269
  IMET route MPLS label: 1046862
  AD route MPLS label: 1040269
  Local ethernet segment:
    ESI: 0000:0000:0000:0183:0184
      Interface: Port-Channel200
      Mode: all-active
      State: down
      ESI label: 1039535
      ES-Import RT: 00:00:18:30:01:84
      DF election state: pending
      Designated forwarder: 
EVPN instance: VLAN-aware bundle 2303-2304
  Route distinguisher: 100.0.0.183:2303
  Route target import: Route-Target-AS:2303:2303
  Route target export: Route-Target-AS:2303:2303
  Service interface: VLAN-aware bundle
  Local MPLS IP address: 100.0.0.183
  VXLAN: disabled
  MPLS: enabled
  Label allocation mode: per-instance
  MAC route MPLS label: 1046830
  IMET route MPLS label: 1039673
  AD route MPLS label: 1046830
  Local ethernet segment:
    ESI: 0000:0000:0000:0183:0184
      Interface: Port-Channel200
      Mode: all-active
      State: down
      ESI label: 1039535
      ES-Import RT: 00:00:18:30:01:84
      DF election state: pending
      Designated forwarder: 
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

 B I      20.10.18.0/24 [200/0] via 100.0.0.18/32, IS-IS SR tunnel index 11, label 1539
                                   via 20.180.183.180, Ethernet1, label 900018
 B I      20.10.21.0/24 [200/0] via 100.0.0.21/32, IS-IS SR tunnel index 9, label 1667
                                   via 20.180.183.180, Ethernet1, label 900021
 B I      20.10.31.0/24 [200/0] via 100.0.0.31/32, IS-IS SR tunnel index 19, label 756641
                                   via 20.180.183.180, Ethernet1, label 900031
 B E      20.10.68.0/24 [20/0] via 100.0.0.184/32, IS-IS SR tunnel index 6, label 132768
                                  via 20.180.183.180, Ethernet1, label 900184
 B I      20.10.108.0/24 [200/0] via 100.0.0.3/32, IS-IS SR tunnel index 5, label 62000
                                    via 20.180.183.180, Ethernet1, label 900003

```

## show interfaces counters rates | nz

```text
Port      Name        Intvl   In Mbps      %  In Kpps  Out Mbps      % Out Kpps
Et1                    5:00       0.6   0.0%        0       0.6   0.0%        0
```

## show running-config section router bgp

```text
router bgp 64512
   router-id 100.0.0.183
   distance bgp 20 200 200
   maximum-paths 4 ecmp 16
   neighbor RR_EVPN peer group
   neighbor RR_EVPN remote-as 64512
   neighbor RR_EVPN next-hop-unchanged
   neighbor RR_EVPN update-source Loopback0
   neighbor RR_EVPN send-community
   neighbor RR_EVPN maximum-routes 12000
   neighbor RR_EVPN-VXLAN peer group
   neighbor RR_EVPN-VXLAN remote-as 64513
   neighbor RR_EVPN-VXLAN next-hop-unchanged
   neighbor RR_EVPN-VXLAN update-source Loopback0
   neighbor RR_EVPN-VXLAN ebgp-multihop 3
   neighbor RR_EVPN-VXLAN send-community
   neighbor bgp peer group
   neighbor bgp rib-in pre-policy retain all
   neighbor 100.0.0.180 peer group RR_EVPN-VXLAN
   neighbor 100.0.0.180 description RR_ANET
   neighbor 100.0.3.58 peer group RR_EVPN
   neighbor 100.0.3.58 description RR_Cisco
   redistribute connected
   !
   vlan 2068
      rd 100.0.0.183:2068
      route-target both 2068:2068
      redistribute learned
      redistribute static
   !
   vlan 2301
      rd 100.0.0.183:2301
      route-target both 2301:2301
      redistribute learned
      redistribute static
   !
   vlan 2302
      rd 100.0.0.183:2302
      route-target both 2302:2302
      redistribute learned
      redistribute static
   !
   vlan-aware-bundle 2303-2304
      rd 100.0.0.183:2303
      route-target both 2303:2303
      redistribute learned
      redistribute static
      vlan 2303-2304
   !
   address-family evpn
      neighbor default encapsulation mpls next-hop-self source-interface Loopback0
      no neighbor RR_EVPN activate
      neighbor RR_EVPN-VXLAN activate
      neighbor RR_EVPN-VXLAN route-map IMPORT-VXLAN-TO-MPLS in
      neighbor RR_EVPN-VXLAN route-map EXPORT-MPLS-TO-VXLAN out
      neighbor RR_EVPN-VXLAN encapsulation mpls next-hop-self source-interface Loopback0
   !
   address-family ipv4
      no neighbor RR_EVPN activate
      no neighbor RR_EVPN-VXLAN activate
   !
   address-family vpn-ipv4
      neighbor RR_EVPN activate
      neighbor RR_EVPN route-map IMPORT-MPLS-TO-VXLAN in
      neighbor RR_EVPN route-map EXPORT-VXLAN-TO-MPLS out
      neighbor default encapsulation mpls next-hop-self source-interface Loopback0
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

## show bgp vpn-ipv4 detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.183, local AS number 64512
BGP routing table entry for IPv4 prefix 20.10.18.0/24, Route Distinguisher: 100.0.0.18:1000
 Paths: 1 available
  Local
    100.0.0.18 from 100.0.3.58 (100.0.3.58)
      Origin INCOMPLETE, metric 0, localpref 100, weight 0, valid, internal, best
      Originator: 100.0.0.21, Cluster list: 100.0.3.58 
      Extended Community: Route-Target-AS:5000:5000
      Remote MPLS label: 1539
BGP routing table entry for IPv4 prefix 20.10.21.0/24, Route Distinguisher: 100.0.0.21:1000
 Paths: 1 available
  Local
    100.0.0.21 from 100.0.3.58 (100.0.3.58)
      Origin INCOMPLETE, metric 0, localpref 100, weight 0, valid, internal, best
      Originator: 100.0.0.21, Cluster list: 100.0.3.58 
      Extended Community: Route-Target-AS:5000:5000
      Remote MPLS label: 1667
BGP routing table entry for IPv4 prefix 20.10.31.0/24, Route Distinguisher: 100.0.0.31:1000
 Paths: 1 available
  Local
    100.0.0.31 from 100.0.3.58 (100.0.3.58)
      Origin IGP, metric -, localpref 100, weight 0, valid, internal, best
      Originator: 100.0.0.31, Cluster list: 100.0.3.58 
      Extended Community: Route-Target-AS:5000:5000
      Remote MPLS label: 756641
BGP routing table entry for IPv4 prefix 20.10.68.0/24, Route Distinguisher: 100.0.0.34:1001
 Paths: 1 available
  Local
    PolicyReject from 100.0.3.58 (100.0.3.58)
      Origin IGP, metric -, localpref -, weight 0, invalid, local
BGP routing table entry for IPv4 prefix 20.10.68.0/24, Route Distinguisher: 100.0.0.183:2000
 Paths: 1 available
  64513 65184
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref 100, weight 0, valid, external, best
      Extended Community: Route-Target-AS:5000:5000
      Rx path id: 0x1
      Local MPLS label (VRF label): 116385
BGP routing table entry for IPv4 prefix 20.10.68.0/24, Route Distinguisher: 100.0.3.41:0
 Paths: 1 available
  Local
    PolicyReject from 100.0.3.58 (100.0.3.58)
      Origin IGP, metric -, localpref -, weight 0, invalid, local
BGP routing table entry for IPv4 prefix 20.10.68.0/24, Route Distinguisher: 100.0.37.9:1000
 Paths: 1 available
  Local
    PolicyReject from 100.0.3.58 (100.0.3.58)
      Origin IGP, metric -, localpref -, weight 0, invalid, local
BGP routing table entry for IPv4 prefix 20.10.68.68/32, Route Distinguisher: 100.0.0.34:1001
 Paths: 1 available
  Local
    PolicyReject from 100.0.3.58 (100.0.3.58)
      Origin IGP, metric -, localpref -, weight 0, invalid, local
BGP routing table entry for IPv4 prefix 20.10.68.68/32, Route Distinguisher: 100.0.3.41:0
 Paths: 1 available
  Local
    PolicyReject from 100.0.3.58 (100.0.3.58)
      Origin IGP, metric -, localpref -, weight 0, invalid, local
BGP routing table entry for IPv4 prefix 20.10.108.0/24, Route Distinguisher: 100.0.0.3:1000
 Paths: 1 available
  Local
    100.0.0.3 from 100.0.3.58 (100.0.3.58)
      Origin INCOMPLETE, metric -, localpref 100, weight 0, valid, internal, best
      Originator: 100.0.0.3, Cluster list: 100.0.3.58 
      Extended Community: Route-Target-AS:5000:5000
      Remote MPLS label: 62000
BGP routing table entry for IPv4 prefix 100.1.37.9/32, Route Distinguisher: 100.0.37.9:1000
 Paths: 1 available
  Local
    100.0.37.9 from 100.0.3.58 (100.0.3.58)
      Origin IGP, metric -, localpref 100, weight 0, valid, internal, best
      Originator: 100.1.37.9, Cluster list: 100.0.3.58 
      Extended Community: Route-Target-AS:1000:1000
      Remote MPLS label: 16
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

