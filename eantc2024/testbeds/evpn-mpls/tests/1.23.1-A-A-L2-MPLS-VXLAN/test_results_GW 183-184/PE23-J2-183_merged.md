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

Uptime: 1 day, 21 hours and 40 minutes
Total memory: 8099732 kB
Free memory: 5083096 kB

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
                           100.0.0.56  4 64512            543       617    0    0 02:21:10 Estab   31     31
  RR_EVPN-VXLAN            100.0.0.180 4 64512           4859      3398    0    0 01:13:25 Estab   79     75
                           100.0.0.184 4 64512           2219      2318    0    0    1d00h Estab   7      4
                           100.0.3.41  4 64512           3130      3704    0    0 03:02:52 Estab   5      5
```

## show bgp evpn instance

```text
EVPN instance: VLAN 3301
  Route distinguisher: 100.0.0.183:3301
  Route distinguisher remote: 100.0.0.183:3301
  Route target import: Route-Target-AS:3301:64512
  Route target export: Route-Target-AS:3301:64512
  Route target import remote: Route-Target-AS:3301:64514
  Route target export remote: Route-Target-AS:3301:64514
  Service interface: VLAN-based
  Local VXLAN IP address: 100.0.0.183
  Local MPLS IP address: 100.0.0.183
  VXLAN: enabled
  MPLS: enabled
  Label allocation mode: per-instance
  MAC route MPLS label: 1036292
  IMET route MPLS label: 1036293
  AD route MPLS label: 1036292
  Remote ethernet segment:
    ESI: 0011:1111:2222:2211:1111
    Active TEPs: 100.0.0.56, 100.0.3.41
  Local ethernet segment:
    ESI: 0000:00d2:0000:0000:00d2
      Interface: MplsTrunk1
      Mode: all-active
      State: up
      ESI label: 1043776
      ES-Import RT: 00:00:d2:00:00:d2
      DF election algorithm: preference
      Designated forwarder: 100.0.0.183
      Non-Designated forwarder: 100.0.0.184
    ESI: 0011:1111:1111:1111:1111
      Interface: Vxlan1
      Mode: all-active
      State: up
      ESI label: 1036288
      ES-Import RT: 11:11:11:11:11:11
      DF election algorithm: preference
      Designated forwarder: 100.0.0.183
      Non-Designated forwarder: 100.0.0.184
EVPN instance: VLAN 3302
  Route distinguisher: 100.0.0.183:3302
  Route distinguisher remote: 100.0.0.183:3302
  Route target import: Route-Target-AS:3302:64512
  Route target export: Route-Target-AS:3302:64512
  Route target import remote: Route-Target-AS:3302:64514
  Route target export remote: Route-Target-AS:3302:64514
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
    ESI: 0000:00d2:0000:0000:00d2
      Interface: MplsTrunk1
      Mode: all-active
      State: up
      ESI label: 1043776
      ES-Import RT: 00:00:d2:00:00:d2
      DF election algorithm: preference
      Designated forwarder: 100.0.0.183
      Non-Designated forwarder: 100.0.0.184
    ESI: 0011:1111:1111:1111:1111
      Interface: Vxlan1
      Mode: all-active
      State: up
      ESI label: 1036288
      ES-Import RT: 11:11:11:11:11:11
      DF election algorithm: preference
      Designated forwarder: 100.0.0.183
      Non-Designated forwarder: 100.0.0.184
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
           via 20.180.183.180, Ethernet1
 I L2     10.0.0.58/32 [115/90]
           via 20.180.183.180, Ethernet1
 I L2     10.0.0.233/32 [115/100]
           via 20.180.183.180, Ethernet1
 I L2     10.0.0.254/32 [115/110]
           via 20.180.183.180, Ethernet1
 I L2     10.0.1.36/32 [115/70]
           via 20.180.183.180, Ethernet1
 I L2     12.0.0.219/32 [115/110]
           via 20.180.183.180, Ethernet1
 I L2     12.0.0.221/32 [115/130]
           via 20.180.183.180, Ethernet1
 I L2     12.0.0.225/32 [115/120]
           via 20.180.183.180, Ethernet1
 I L2     12.0.0.227/32 [115/120]
           via 20.180.183.180, Ethernet1
 I L2     20.3.180.0/24 [115/20]
           via 20.180.183.180, Ethernet1
 I L2     20.18.180.0/24 [115/20]
           via 20.180.183.180, Ethernet1
 I L2     20.21.180.0/24 [115/20]
           via 20.180.183.180, Ethernet1
 I L2     20.26.180.0/24 [115/20]
           via 20.180.183.180, Ethernet1
 I L2     20.31.180.0/24 [115/20]
           via 20.180.183.180, Ethernet1
 I L2     20.34.180.0/24 [115/20]
           via 20.180.183.180, Ethernet1
 I L2     20.52.1.0/24 [115/120]
           via 20.180.183.180, Ethernet1
 I L2     20.54.2.0/24 [115/110]
           via 20.180.183.180, Ethernet1
 I L2     20.55.2.0/24 [115/90]
           via 20.180.183.180, Ethernet1
 I L2     20.56.2.0/24 [115/110]
           via 20.180.183.180, Ethernet1
 I L2     20.56.180.0/24 [115/20]
           via 20.180.183.180, Ethernet1
 I L2     20.57.10.0/24 [115/90]
           via 20.180.183.180, Ethernet1
 I L2     20.57.11.0/24 [115/90]
           via 20.180.183.180, Ethernet1
 I L2     20.57.13.0/24 [115/110]
           via 20.180.183.180, Ethernet1
 I L2     20.57.14.0/24 [115/110]
           via 20.180.183.180, Ethernet1
 I L2     20.57.15.0/24 [115/110]
           via 20.180.183.180, Ethernet1
 I L2     20.161.180.0/24 [115/20]
           via 20.180.183.180, Ethernet1
 I L2     20.180.181.0/24 [115/20]
           via 20.180.183.180, Ethernet1
 I L2     20.180.182.0/24 [115/20]
           via 20.180.183.180, Ethernet1
 C        20.180.183.0/24
           directly connected, Ethernet1
 I L2     20.180.184.0/24 [115/20]
           via 20.180.183.180, Ethernet1
 I L2     20.219.225.0/24 [115/90]
           via 20.180.183.180, Ethernet1
 I L2     25.20.225.0/24 [115/90]
           via 20.180.183.180, Ethernet1
 I L2     25.29.225.0/24 [115/90]
           via 20.180.183.180, Ethernet1
 I L2     25.36.225.0/24 [115/90]
           via 20.180.183.180, Ethernet1
 I L2     25.58.225.0/24 [115/90]
           via 20.180.183.180, Ethernet1
 I L2     25.59.225.0/24 [115/90]
           via 20.180.183.180, Ethernet1
 I L2     25.102.225.0/24 [115/90]
           via 20.180.183.180, Ethernet1
 I L2     25.107.225.0/24 [115/90]
           via 20.180.183.180, Ethernet1
 I L2     25.110.225.0/24 [115/90]
           via 20.180.183.180, Ethernet1
 I L2     25.116.225.0/24 [115/90]
           via 20.180.183.180, Ethernet1
 I L2     25.136.225.0/24 [115/90]
           via 20.180.183.180, Ethernet1
 I L2     25.138.225.0/24 [115/90]
           via 20.180.183.180, Ethernet1
 I L2     25.142.225.0/24 [115/90]
           via 20.180.183.180, Ethernet1
 I L2     25.144.225.0/24 [115/90]
           via 20.180.183.180, Ethernet1
 I L2     25.152.225.0/24 [115/90]
           via 20.180.183.180, Ethernet1
 I L2     25.153.225.0/24 [115/90]
           via 20.180.183.180, Ethernet1
 I L2     30.9.180.0/24 [115/20]
           via 20.180.183.180, Ethernet1
 I L2     30.14.180.0/24 [115/20]
           via 20.180.183.180, Ethernet1
 I L2     30.41.180.0/24 [115/20]
           via 20.180.183.180, Ethernet1
 I L2     30.45.180.0/24 [115/20]
           via 20.180.183.180, Ethernet1
 I L2     30.48.180.0/24 [115/20]
           via 20.180.183.180, Ethernet1
 I L2     30.58.180.0/24 [115/20]
           via 20.180.183.180, Ethernet1
 I L2     30.60.180.0/24 [115/20]
           via 20.180.183.180, Ethernet1
 I L2     30.79.180.0/24 [115/20]
           via 20.180.183.180, Ethernet1
 I L2     100.0.0.3/32 [115/30]
           via 20.180.183.180, Ethernet1
 I L2     100.0.0.18/32 [115/20]
           via 20.180.183.180, Ethernet1
 I L2     100.0.0.21/32 [115/20]
           via 20.180.183.180, Ethernet1
 I L2     100.0.0.26/32 [115/20]
           via 20.180.183.180, Ethernet1
 I L2     100.0.0.31/32 [115/20]
           via 20.180.183.180, Ethernet1
 I L2     100.0.0.34/32 [115/20]
           via 20.180.183.180, Ethernet1
 I L2     100.0.0.56/32 [115/20]
           via 20.180.183.180, Ethernet1
 I L2     100.0.0.161/32 [115/30]
           via 20.180.183.180, Ethernet1
 I L2     100.0.0.180/32 [115/10]
           via 20.180.183.180, Ethernet1
 I L2     100.0.0.181/32 [115/30]
           via 20.180.183.180, Ethernet1
 I L2     100.0.0.182/32 [115/20]
           via 20.180.183.180, Ethernet1
 C        100.0.0.183/32
           directly connected, Loopback0
 I L2     100.0.0.184/32 [115/20]
           via 20.180.183.180, Ethernet1
 I L2     100.0.3.41/32 [115/30]
           via 20.180.183.180, Ethernet1
 I L2     100.0.3.45/32 [115/30]
           via 20.180.183.180, Ethernet1
 I L2     100.0.3.48/32 [115/30]
           via 20.180.183.180, Ethernet1
 I L2     100.0.3.58/32 [115/30]
           via 20.180.183.180, Ethernet1
 I L2     100.0.3.60/32 [115/30]
           via 20.180.183.180, Ethernet1
 I L2     100.0.30.9/32 [115/20]
           via 20.180.183.180, Ethernet1
 I L2     100.0.37.9/32 [115/20]
           via 20.180.183.180, Ethernet1
 I L2     192.168.20.0/23 [115/20]
           via 20.180.183.180, Ethernet1


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

 B I      30.30.1.0/24 [200/0]
           via VTEP 100.0.0.181 VNI 1023 router-mac 28:99:3a:8f:8f:6f
 B I      30.30.2.0/24 [200/0]
           via VTEP 100.0.0.181 VNI 1023 router-mac 28:99:3a:8f:8f:6f
 B I      30.30.5.0/24 [200/0]
           via 100.0.3.41/32, IS-IS SR tunnel index 9, label 24006
              via 20.180.183.180, Ethernet1, label 900341
 C        100.0.181.181/32
           directly connected, Loopback100


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

 C        192.168.20.0/24
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


```

## show interfaces counters rates | nz

```text
Port      Name      Intvl  In Mbps      %  In Kpps Out Mbps      % Out Kpps
Et1                  5:00      0.3   0.0%        0      0.2   0.0%        0
```

## show running-config section router bgp

```text
router bgp 64512
   router-id 100.0.0.183
   distance bgp 20 200 200
   maximum-paths 4 ecmp 16
   bgp bestpath d-path
   bgp bestpath skip next-hop igp-cost
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
   neighbor 100.0.0.56 peer group RR_EVPN
   neighbor 100.0.0.180 peer group RR_EVPN-VXLAN
   neighbor 100.0.0.180 description RR_EVPN-VXLAN
   neighbor 100.0.0.184 peer group RR_EVPN
   neighbor 100.0.3.41 peer group RR_EVPN
   redistribute connected
   !
   vlan 3301
      rd evpn domain all 100.0.0.183:3301
      route-target import export 3301:64512
      route-target import export evpn domain remote 3301:64514
      redistribute learned
      redistribute static
   !
   vlan 3302
      rd evpn domain all 100.0.0.183:3302
      route-target import export 3302:64512
      route-target import export evpn domain remote 3302:64514
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
      domain identifier 1:1
      domain identifier 1:2 remote
      layer-2 fec in-place update
      !
      evpn ethernet-segment domain local
         identifier 0011:1111:1111:1111:1111
         designated-forwarder election algorithm preference 150
         route-target import 11:11:11:11:11:11
      !
      evpn ethernet-segment domain remote
         identifier 0000:00d2:0000:0000:00d2
         designated-forwarder election algorithm preference 150
         route-target import 00:00:d2:00:00:d2
   !
   address-family ipv4
      no neighbor RR_EVPN activate
      no neighbor RR_EVPN-VXLAN activate
   !
   vrf L2GW
      rd 100.0.0.183:1023
      rd evpn domain remote 100.0.0.183:1023
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
0     524263 MPLS  0000.0206.0206     100.0.0.56         Stic
                                                         ky  
0     24000  MPLS  0000.0206.0206     100.0.3.41         Stic
                                                         ky  
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
| 3301| 00:00:02:06:02:06 |         FEC| 0x00001 | 0 | N | Y | N  |    MplsTrunk1|
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
|1    |131074|ROUTE| FEC 183510         |   - |2097150 |                 - |Mpush 900341 24000
|1    |131075|ROUTE| FEC 183510         |   - |2097149 |                 - |Mpush 900056 524263
|  -  |131072|ROUTE| FEC 183511         |4093 |103425  | 28:99:3a:8f:8f:6f |   -   
|  -  |131073|ROUTE| FEC 183510         |   - |2097151 |                 - |Mpush 900341 24006
|  -  |183502|DROP | DROP               |0    |  -     |                   |   -   
|  -  |183503|ROUTE| Et1                |1006 |103421  | 44:4c:a8:73:9c:0d |   -   
|  -  |183504|DROP | DROP               |0    |  -     |                   |   -   
|  -  |183505|DROP | DROP               |0    |  -     |                   |   -   
|  -  |183506|ROUTE| Et1                |1006 |103421  | 44:4c:a8:73:9c:0d |   -   
|  -  |183507|ROUTE| Et1                |1006 |103421  | 44:4c:a8:73:9c:0d |   -   
|  -  |183509|DROP | DROP               |0    |  -     |                   |   -   
|  -  |183510|ROUTE| Et1                |1006 |103421  | 44:4c:a8:73:9c:0d |   -   
|  -  |183511|ROUTE| Et1                |1006 |103423  | 44:4c:a8:73:9c:0d |T 100.0.0.181
|  -  |314667|TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |   -   
|  -  |314670|TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |   -   
|  -  |314671|TRAP | CoppSystemL3LpmOver|0    |  -     | SlowReceive       |   -   
|  -  |314672|TRAP | CoppSystemL3LpmOver|0    |  -     | SlowReceive       |   -   
|  -  |314673|TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |   -   
|  -  |315679|TRAP | CoppSystemL3DstMiss|1006 |1006    | ArpTrap           |   -   

```

