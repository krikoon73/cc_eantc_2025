# Test results for PE21-J2-206

## show version

```text
Arista DCS-7050SX3-48YC12-F
Hardware version: 11.03
Serial number: JPE19101105
Hardware MAC address: 985d.82c4.0271
System MAC address: 985d.82c4.0271

Software image version: 4.31.2F
Architecture: x86_64
Internal build version: 4.31.2F-35442176.4312F
Internal build ID: 500c58e3-5beb-4481-afe9-8ad77245cc44
Image format version: 3.0
Image optimization: Default

Uptime: 3 days, 7 hours and 34 minutes
Total memory: 8051592 kB
Free memory: 5550556 kB

```

## show interfaces status

```text
Port       Name       Status       Vlan     Duplex Speed  Type         Flags Encapsulation
Et1                   disabled     routed   full   10G    10GBASE-LR                     
Et2                   notconnect   routed   full   10G    Not Present                    
Et3                   notconnect   routed   full   10G    Not Present                    
Et4                   notconnect   routed   full   10G    Not Present                    
Et5                   disabled     routed   auto   auto   10GBASE-T                      
Et6                   disabled     routed   full   10G    10GBASE-LR                     
Et7                   notconnect   routed   full   10G    Not Present                    
Et8                   notconnect   routed   full   10G    Not Present                    
Et9                   notconnect   routed   full   10G    Not Present                    
Et10                  connected    trunk    full   10G    10GBASE-SRL                    
Et11                  notconnect   routed   full   10G    Not Present                    
Et12                  notconnect   routed   full   10G    Not Present                    
Et13                  notconnect   routed   full   10G    Not Present                    
Et14                  notconnect   routed   full   10G    Not Present                    
Et15                  notconnect   routed   full   10G    Not Present                    
Et16                  notconnect   routed   full   10G    Not Present                    
Et17                  notconnect   routed   full   10G    Not Present                    
Et18                  notconnect   routed   full   10G    Not Present                    
Et19                  notconnect   routed   full   10G    Not Present                    
Et20                  notconnect   routed   full   10G    Not Present                    
Et21                  notconnect   routed   full   10G    Not Present                    
Et22                  notconnect   routed   full   10G    Not Present                    
Et23                  notconnect   routed   full   10G    Not Present                    
Et24                  notconnect   routed   full   10G    Not Present                    
Et25                  notconnect   routed   full   10G    Not Present                    
Et26                  notconnect   routed   full   10G    Not Present                    
Et27                  notconnect   routed   full   10G    Not Present                    
Et28                  notconnect   routed   full   10G    Not Present                    
Et29                  notconnect   routed   full   10G    Not Present                    
Et30                  notconnect   routed   full   10G    Not Present                    
Et31                  notconnect   routed   full   10G    Not Present                    
Et32                  notconnect   routed   full   10G    Not Present                    
Et33                  notconnect   routed   full   10G    Not Present                    
Et34                  notconnect   routed   full   10G    Not Present                    
Et35                  notconnect   routed   full   10G    Not Present                    
Et36                  notconnect   routed   full   10G    Not Present                    
Et37                  notconnect   routed   full   10G    Not Present                    
Et38                  notconnect   routed   full   10G    Not Present                    
Et39                  notconnect   routed   full   10G    Not Present                    
Et40                  notconnect   routed   full   10G    Not Present                    
Et41                  notconnect   routed   full   10G    Not Present                    
Et42                  notconnect   routed   full   10G    Not Present                    
Et43                  notconnect   routed   full   10G    Not Present                    
Et44                  notconnect   routed   full   10G    Not Present                    
Et45                  notconnect   routed   full   10G    Not Present                    
Et46                  notconnect   routed   full   10G    Not Present                    
Et47                  notconnect   routed   full   10G    Not Present                    
Et48                  notconnect   routed   full   10G    Not Present                    
Et49/1                connected    routed   full   10G    40GBASE-SR4                    
Et49/2     ANET-SPINE connected    routed   full   10G    40GBASE-SR4                    
Et49/3                connected    routed   full   10G    40GBASE-SR4                    
Et49/4                connected    routed   full   10G    40GBASE-SR4                    
Et50/1                notconnect   routed   full   100G   Not Present                    
Et51/1                notconnect   routed   full   100G   Not Present                    
Et52/1                notconnect   routed   full   100G   Not Present                    
Et53/1                notconnect   routed   full   100G   Not Present                    
Et54/1                notconnect   routed   full   100G   Not Present                    
Et55/1                notconnect   routed   full   100G   Not Present                    
Et56/1                notconnect   routed   full   100G   Not Present                    
Et57/1                notconnect   routed   full   100G   Not Present                    
Et58/1                notconnect   routed   full   100G   Not Present                    
Et59/1                notconnect   routed   full   100G   Not Present                    
Et60/1                notconnect   routed   full   100G   Not Present                    
Ma1                   connected    routed   a-full a-1G   10/100/1000                    

```

## show bgp evpn summary

```text
BGP summary information for VRF default
Router identifier 100.0.0.206, local AS number 65206
Neighbor Status Codes: m - Under maintenance
  Description              Neighbor    V AS           MsgRcvd   MsgSent  InQ OutQ  Up/Down State   PfxRcd PfxAcc
  EVPN-SPINE               100.0.0.200 4 65000           7020      1679    0    0 23:14:02 Estab   176    176
```

## show bgp evpn instance

```text
EVPN instance: VLAN 3301
  Route distinguisher: 100.0.0.206:3301
  Route target import: Route-Target-AS:3301:3301
  Route target export: Route-Target-AS:3301:3301
  Service interface: VLAN-based
  Local VXLAN IP address: 100.0.0.206
  VXLAN: enabled
  MPLS: disabled
  Remote ethernet segment:
    ESI: 0011:1111:2222:2211:1111
    Active TEPs: 100.0.3.41
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

 B E      20.41.200.0/24 [20/0]
           via 20.200.206.200, Ethernet49/2
 B E      20.56.200.0/24 [20/0]
           via 20.200.206.200, Ethernet49/2
 C        20.200.206.0/24
           directly connected, Ethernet49/2
 B E      100.0.0.56/32 [20/0]
           via 20.200.206.200, Ethernet49/2
 B E      100.0.0.200/32 [20/0]
           via 20.200.206.200, Ethernet49/2
 C        100.0.0.206/32
           directly connected, Loopback0
 B E      100.0.3.41/32 [20/0]
           via 20.200.206.200, Ethernet49/2


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

 B E      30.30.1.0/24 [20/0]
           via VTEP 100.0.3.41 VNI 1000 router-mac f8:7a:41:6d:d0:f0
 B E      30.30.2.0/24 [20/0]
           via VTEP 100.0.3.41 VNI 1000 router-mac f8:7a:41:6d:d0:f0
 C        30.30.5.0/24
           directly connected, Vlan3305


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

! IP routing not enabled

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

 C        10.10.206.0/24
           directly connected, Vlan1206
 C        30.30.1.0/24
           directly connected, Vlan3301

```

## show interfaces counters rates | nz

```text
Port      Name       Intvl  In Mbps      %  In Kpps Out Mbps      % Out Kpps
```

## show running-config section router bgp

```text
router bgp 65206
   router-id 100.0.0.206
   distance bgp 20 200 200
   maximum-paths 128
   neighbor EVPN-IPV4-SPINE peer group
   neighbor EVPN-IPV4-SPINE remote-as 65000
   neighbor EVPN-IPV4-SPINE update-source Loopback0
   neighbor EVPN-IPV4-SPINE ebgp-multihop 5
   neighbor EVPN-IPV4-SPINE send-community extended
   neighbor IPV4-SPINE peer group
   neighbor IPV4-SPINE remote-as 65000
   neighbor IPV4-SPINE ebgp-multihop 5
   neighbor 20.200.206.200 peer group IPV4-SPINE
   neighbor 20.200.206.200 description IPV4-SPINE
   neighbor 100.0.0.200 peer group EVPN-IPV4-SPINE
   neighbor 100.0.0.200 description EVPN-SPINE
   redistribute connected
   !
   vlan 3301
      rd 100.0.0.206:3301
      route-target both 3301:3301
      redistribute learned
      redistribute static
   !
   address-family evpn
      neighbor EVPN-IPV4-SPINE activate
   !
   address-family ipv4
      no neighbor EVPN-IPV4-SPINE activate
   !
   vrf L2GW
      rd 100.0.0.206:1023
      route-target import evpn 1023:1023
      route-target export evpn 1023:1023
      redistribute connected
```

## show running-config section interfaces

```text
```

