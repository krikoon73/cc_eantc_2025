# Test results for PE21-J2-181

## show version

```text
Arista DCS-7280SR2A-48YC6-F
Hardware version: 20.04
Serial number: SSJ17095073
Hardware MAC address: 2899.3a8f.8f6f
System MAC address: 2899.3a8f.8f6f

Software image version: 4.32.0F-35483270.hudsonrel (engineering build)
Architecture: x86_64
Internal build version: 4.32.0F-35483270.hudsonrel
Internal build ID: bc4c8e97-b142-4c39-a634-2b265e10ac86
Image format version: 3.0
Image optimization: Sand-4GB

Uptime: 3 days, 6 hours and 26 minutes
Total memory: 8051592 kB
Free memory: 4927420 kB

```

## show interfaces status

```text
! * Incomplete encapsulation information. Use 'show interface encapsulation vlan' instead
Port       Name   Status       Vlan     Duplex Speed  Type         Flags Encapsulation
Et1               connected    routed   full   10G    10GBASE-SRL                    
Et2               errdisabled  1        full   25G    Not Present                    
Et3               errdisabled  1        full   25G    Not Present                    
Et4               errdisabled  1        full   25G    Not Present                    
Et5               connected    trunk    full   10G    10GBASE-SRL                    
Et5.2320          notconnect   routed   full   10G    subinterface       *           
Et5.2321          notconnect   routed   full   10G    subinterface       *           
Et6               errdisabled  1        full   25G    Not Present                    
Et7               errdisabled  1        full   25G    Not Present                    
Et8               errdisabled  1        full   25G    Not Present                    
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
Et41              notconnect   1        full   25G    Not Present                    
Et42              notconnect   1        full   25G    Not Present                    
Et43              notconnect   1        full   25G    Not Present                    
Et44              notconnect   1        full   25G    Not Present                    
Et45              notconnect   1        full   25G    Not Present                    
Et46              notconnect   1        full   25G    Not Present                    
Et47              notconnect   1        full   25G    Not Present                    
Et48              notconnect   1        full   25G    Not Present                    
Et49/1            notconnect   1        full   100G   Not Present                    
Et50/1            notconnect   1        full   100G   Not Present                    
Et51/1            notconnect   1        full   100G   Not Present                    
Et52/1            notconnect   1        full   100G   Not Present                    
Et53/1            notconnect   1        full   100G   Not Present                    
Et54/1            notconnect   1        full   100G   Not Present                    
Ma1               connected    routed   a-full a-1G   10/100/1000                    
Po100             notconnect   trunk    full   unconf N/A                            
Po419             notconnect   routed   full   unconf N/A                            
Po419.2310        notconnect   routed   full   unconf subinterface       *           

```

## show bgp evpn summary

```text
BGP summary information for VRF default
Router identifier 100.0.0.181, local AS number 64512
Neighbor Status Codes: m - Under maintenance
  Neighbor    V AS           MsgRcvd   MsgSent  InQ OutQ  Up/Down State   PfxRcd PfxAcc
  100.0.0.180 4 64512           9844      4607    0    0 01:28:30 Estab   87     87
```

## show bgp evpn instance

```text
EVPN instance: VLAN 2181
  Route distinguisher: 100.0.0.181:2181
  Route target import: Route-Target-AS:2181:2181
  Route target export: Route-Target-AS:2181:2181
  Service interface: VLAN-based
  Local VXLAN IP address: 100.0.0.181
  VXLAN: enabled
  MPLS: disabled
  Local ethernet segment:
    ESI: 0000:0000:0000:0181:0182
      Interface: Port-Channel100
      Mode: all-active
      State: down
      ES-Import RT: 00:00:18:10:01:82
      DF election state: pending
      Designated forwarder: 
EVPN instance: VLAN 3301
  Route distinguisher: 100.0.0.181:3301
  Route target import: Route-Target-AS:3301:64512
  Route target export: Route-Target-AS:3301:64512
  Service interface: VLAN-based
  Local VXLAN IP address: 100.0.0.181
  VXLAN: enabled
  MPLS: disabled
  Remote ethernet segment:
    ESI: 0000:00d2:0000:0000:00d2
    Active TEPs: 100.0.0.183, 100.0.0.184
EVPN instance: VLAN 3302
  Route distinguisher: 100.0.0.181:3302
  Route target import: Route-Target-AS:3302:64512
  Route target export: Route-Target-AS:3302:64512
  Service interface: VLAN-based
  Local VXLAN IP address: 100.0.0.181
  VXLAN: enabled
  MPLS: disabled
  Remote ethernet segment:
    ESI: 0000:00d2:0000:0000:00d2
    Active TEPs: 100.0.0.183, 100.0.0.184
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

 I L2     10.0.0.57/32 [115/100]
           via 20.180.181.180, Ethernet1
 I L2     10.0.0.58/32 [115/90]
           via 20.180.181.180, Ethernet1
 I L2     10.0.0.233/32 [115/100]
           via 20.180.181.180, Ethernet1
 I L2     10.0.0.254/32 [115/110]
           via 20.180.181.180, Ethernet1
 I L2     10.0.1.36/32 [115/70]
           via 20.180.181.180, Ethernet1
 I L2     12.0.0.219/32 [115/110]
           via 20.180.181.180, Ethernet1
 I L2     12.0.0.221/32 [115/130]
           via 20.180.181.180, Ethernet1
 I L2     12.0.0.225/32 [115/120]
           via 20.180.181.180, Ethernet1
 I L2     12.0.0.227/32 [115/120]
           via 20.180.181.180, Ethernet1
 I L2     20.3.180.0/24 [115/20]
           via 20.180.181.180, Ethernet1
 I L2     20.18.180.0/24 [115/20]
           via 20.180.181.180, Ethernet1
 I L2     20.21.180.0/24 [115/20]
           via 20.180.181.180, Ethernet1
 I L2     20.26.180.0/24 [115/20]
           via 20.180.181.180, Ethernet1
 I L2     20.31.180.0/24 [115/20]
           via 20.180.181.180, Ethernet1
 I L2     20.34.180.0/24 [115/20]
           via 20.180.181.180, Ethernet1
 I L2     20.52.1.0/24 [115/120]
           via 20.180.181.180, Ethernet1
 I L2     20.54.2.0/24 [115/110]
           via 20.180.181.180, Ethernet1
 I L2     20.55.2.0/24 [115/90]
           via 20.180.181.180, Ethernet1
 I L2     20.56.2.0/24 [115/110]
           via 20.180.181.180, Ethernet1
 I L2     20.56.180.0/24 [115/20]
           via 20.180.181.180, Ethernet1
 I L2     20.57.10.0/24 [115/90]
           via 20.180.181.180, Ethernet1
 I L2     20.57.11.0/24 [115/90]
           via 20.180.181.180, Ethernet1
 I L2     20.57.13.0/24 [115/110]
           via 20.180.181.180, Ethernet1
 I L2     20.57.14.0/24 [115/110]
           via 20.180.181.180, Ethernet1
 I L2     20.57.15.0/24 [115/110]
           via 20.180.181.180, Ethernet1
 I L2     20.161.180.0/24 [115/20]
           via 20.180.181.180, Ethernet1
 C        20.180.181.0/24
           directly connected, Ethernet1
 I L2     20.180.182.0/24 [115/20]
           via 20.180.181.180, Ethernet1
 I L2     20.180.183.0/24 [115/20]
           via 20.180.181.180, Ethernet1
 I L2     20.180.184.0/24 [115/20]
           via 20.180.181.180, Ethernet1
 I L2     25.29.225.0/24 [115/90]
           via 20.180.181.180, Ethernet1
 I L2     25.36.225.0/24 [115/90]
           via 20.180.181.180, Ethernet1
 I L2     25.58.225.0/24 [115/90]
           via 20.180.181.180, Ethernet1
 I L2     25.59.225.0/24 [115/90]
           via 20.180.181.180, Ethernet1
 I L2     25.102.225.0/24 [115/90]
           via 20.180.181.180, Ethernet1
 I L2     25.107.225.0/24 [115/90]
           via 20.180.181.180, Ethernet1
 I L2     25.110.225.0/24 [115/90]
           via 20.180.181.180, Ethernet1
 I L2     25.116.225.0/24 [115/90]
           via 20.180.181.180, Ethernet1
 I L2     25.136.225.0/24 [115/90]
           via 20.180.181.180, Ethernet1
 I L2     25.138.225.0/24 [115/90]
           via 20.180.181.180, Ethernet1
 I L2     25.142.225.0/24 [115/90]
           via 20.180.181.180, Ethernet1
 I L2     25.144.225.0/24 [115/90]
           via 20.180.181.180, Ethernet1
 I L2     25.152.225.0/24 [115/90]
           via 20.180.181.180, Ethernet1
 I L2     25.153.225.0/24 [115/90]
           via 20.180.181.180, Ethernet1
 I L2     30.9.180.0/24 [115/20]
           via 20.180.181.180, Ethernet1
 I L2     30.14.180.0/24 [115/20]
           via 20.180.181.180, Ethernet1
 I L2     30.41.180.0/24 [115/20]
           via 20.180.181.180, Ethernet1
 I L2     30.45.180.0/24 [115/20]
           via 20.180.181.180, Ethernet1
 I L2     30.48.180.0/24 [115/20]
           via 20.180.181.180, Ethernet1
 I L2     30.58.180.0/24 [115/20]
           via 20.180.181.180, Ethernet1
 I L2     30.60.180.0/24 [115/20]
           via 20.180.181.180, Ethernet1
 I L2     30.79.180.0/24 [115/20]
           via 20.180.181.180, Ethernet1
 I L2     100.0.0.3/32 [115/30]
           via 20.180.181.180, Ethernet1
 I L2     100.0.0.18/32 [115/20]
           via 20.180.181.180, Ethernet1
 I L2     100.0.0.21/32 [115/20]
           via 20.180.181.180, Ethernet1
 I L2     100.0.0.26/32 [115/20]
           via 20.180.181.180, Ethernet1
 I L2     100.0.0.31/32 [115/20]
           via 20.180.181.180, Ethernet1
 I L2     100.0.0.34/32 [115/20]
           via 20.180.181.180, Ethernet1
 I L2     100.0.0.56/32 [115/20]
           via 20.180.181.180, Ethernet1
 I L2     100.0.0.161/32 [115/30]
           via 20.180.181.180, Ethernet1
 I L2     100.0.0.180/32 [115/10]
           via 20.180.181.180, Ethernet1
 C        100.0.0.181/32
           directly connected, Loopback0
 I L2     100.0.0.182/32 [115/20]
           via 20.180.181.180, Ethernet1
 I L2     100.0.0.183/32 [115/20]
           via 20.180.181.180, Ethernet1
 I L2     100.0.0.184/32 [115/20]
           via 20.180.181.180, Ethernet1
 I L2     100.0.3.41/32 [115/30]
           via 20.180.181.180, Ethernet1
 I L2     100.0.3.45/32 [115/30]
           via 20.180.181.180, Ethernet1
 I L2     100.0.3.48/32 [115/30]
           via 20.180.181.180, Ethernet1
 I L2     100.0.3.58/32 [115/30]
           via 20.180.181.180, Ethernet1
 I L2     100.0.3.60/32 [115/30]
           via 20.180.181.180, Ethernet1
 I L2     100.0.30.9/32 [115/20]
           via 20.180.181.180, Ethernet1
 I L2     100.0.37.9/32 [115/20]
           via 20.180.181.180, Ethernet1
 I L2     192.168.20.0/23 [115/20]
           via 20.180.181.180, Ethernet1


VRF: L2GW
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

 C        30.30.1.0/24
           directly connected, Vlan3301
 C        30.30.2.0/24
           directly connected, Vlan3302
 B I      30.30.5.0/24 [200/0]
           via VTEP 100.0.0.183 VNI 1023 router-mac c4:ca:2b:45:ef:6d
           via VTEP 100.0.0.184 VNI 1023 router-mac c4:ca:2b:45:e7:39


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



VRF: tenant-d
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


! IP routing not enabled
```

## show interfaces counters rates | nz

```text
Port      Name      Intvl  In Mbps      %  In Kpps Out Mbps      % Out Kpps
```

## show running-config section router bgp

```text
router bgp 64512
   router-id 100.0.0.181
   distance bgp 20 200 200
   maximum-paths 8 ecmp 16
   neighbor RR_EVPN peer group
   neighbor RR_EVPN remote-as 64512
   neighbor RR_EVPN next-hop-unchanged
   neighbor RR_EVPN update-source Loopback0
   neighbor RR_EVPN send-community extended
   neighbor RR_EVPN maximum-routes 12000
   neighbor 100.0.0.180 peer group RR_EVPN
   redistribute connected
   !
   vlan 2181
      rd 100.0.0.181:2181
      route-target both 2181:2181
      redistribute learned
      redistribute static
   !
   vlan 3301
      rd 100.0.0.181:3301
      route-target both 3301:64512
      redistribute learned
      redistribute static
   !
   vlan 3302
      rd 100.0.0.181:3302
      route-target both 3302:64512
      redistribute learned
      redistribute static
   !
   address-family evpn
      neighbor default encapsulation mpls next-hop-self source-interface Loopback0
      neighbor RR_EVPN activate
      neighbor RR_EVPN encapsulation vxlan 
   !
   address-family ipv4
      no neighbor RR_EVPN activate
   !
   vrf L2GW
      rd 100.0.0.181:1023
      route-target import evpn 1023:1023
      route-target export evpn 1023:1023
      maximum-paths 4 ecmp 4
      redistribute connected
   !
   vrf tenant-a
      rd 100.0.0.181:2000
      evpn multicast
      route-target import evpn 2000:2000
      route-target export evpn 2000:2000
      redistribute connected
```

## show running-config section interfaces

```text
alias d show interfaces description | grep -v 'not\|down'
```

