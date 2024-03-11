# Test results for Spine2-J-180

## show version

```text
Arista DCS-7280SR-48C6-F
Hardware version: 01.02
Serial number: JPE16200927
Hardware MAC address: 444c.a873.9c0d
System MAC address: 444c.a873.9c0d

Software image version: 4.28.0F
Architecture: i686
Internal build version: 4.28.0F-26924507.4280F
Internal build ID: cc8af7a4-3c5b-4f00-bf78-68394d62ceff
Image format version: 3.0
Image optimization: Sand-4GB

Uptime: 1 day, 6 hours and 36 minutes
Total memory: 8098968 kB
Free memory: 6042440 kB

```

## show interfaces status

```text
Port       Name            Status       Vlan     Duplex Speed  Type         Flags Encapsulation
Et1        PE21-J2-181     connected    routed   full   10G    10GBASE-SRL                    
Et2                        connected    routed   full   10G    10GBASE-SRL                    
Et3        PE23-J2-183     connected    routed   full   10G    10GBASE-SRL                    
Et4        PE24-J2-184     connected    routed   full   10G    10GBASE-SRL                    
Et5                        notconnect   1        full   10G    Not Present                    
Et6                        notconnect   1        full   10G    Not Present                    
Et7                        notconnect   1        full   10G    Not Present                    
Et8        h3c_21          connected    routed   full   10G    10GBASE-SRL                    
Et9        Huawei-34       connected    routed   full   10G    10GBASE-SRL                    
Et10       H3C-18          connected    routed   full   10G    10GBASE-SRL                    
Et11       Nokia           connected    routed   full   10G    10GBASE-SRL                    
Et12       Ciena-3         connected    routed   full   10G    10GBASE-SRL                    
Et13                       notconnect   1        full   10G    Not Present                    
Et14                       notconnect   1        full   10G    Not Present                    
Et15       rbbn-31         connected    routed   full   10G    10GBASE-SRL                    
Et16                       notconnect   1        full   10G    Not Present                    
Et17       Cisco-ASR9K-341 connected    routed   full   10G    10GBASE-SRL                    
Et18       Cisco-NCS5K-345 connected    routed   full   10G    10GBASE-SRL                    
Et19       Cisco-NCS5K-48  connected    routed   full   10G    10GBASE-SRL                    
Et20       Cisco-8K-54     notconnect   routed   full   10G    10GBASE-AR                     
Et21       Cisco-NCS57-45  connected    routed   full   10G    10GBASE-SRL                    
Et22                       notconnect   1        full   10G    Not Present                    
Et23       H3C-26          connected    routed   full   10G    10GBASE-SRL                    
Et24       H3C-27          notconnect   routed   full   10G    10GBASE-SRL                    
Et25       Jnpr-ACX-309    connected    routed   full   10G    10GBASE-SR                     
Et26       Jnpr-ACX314     connected    routed   full   10G    10GBASE-SR                     
Et27       Cisco-VM        connected    routed   full   10G    10GBASE-LR                     
Et28                       notconnect   1        full   10G    Not Present                    
Et29                       notconnect   1        full   10G    Not Present                    
Et30                       notconnect   1        full   10G    Not Present                    
Et31                       notconnect   1        full   10G    Not Present                    
Et32                       notconnect   1        full   10G    Not Present                    
Et33                       notconnect   1        full   10G    Not Present                    
Et34                       notconnect   1        full   10G    Not Present                    
Et35                       notconnect   1        full   10G    Not Present                    
Et36                       notconnect   1        full   10G    Not Present                    
Et37                       notconnect   1        full   10G    Not Present                    
Et38                       notconnect   1        full   10G    Not Present                    
Et39                       notconnect   1        full   10G    Not Present                    
Et40                       notconnect   1        full   10G    Not Present                    
Et41                       notconnect   1        full   10G    Not Present                    
Et42                       notconnect   1        full   10G    Not Present                    
Et43                       notconnect   1        full   10G    Not Present                    
Et44                       notconnect   routed   full   10G    10GBASE-AR                     
Et45                       notconnect   1        full   10G    Not Present                    
Et46                       notconnect   1        full   10G    Not Present                    
Et47                       notconnect   1        full   10G    Not Present                    
Et48                       connected    routed   full   10G    10GBASE-LR                     
Et49/1     Jnpr-MX304-379  connected    routed   full   100G   100GBASE-LR4                   
Et50/1                     notconnect   1        full   100G   100GBASE-SR4                   
Et51/1                     notconnect   1        full   100G   Not Present                    
Et52/1                     notconnect   1        full   100G   Not Present                    
Et53/1                     notconnect   1        full   100G   Not Present                    
Et54/1                     notconnect   1        full   100G   Not Present                    
Ma1                        connected    routed   a-full a-1G   10/100/1000                    

```

## show bgp evpn summary

```text
BGP summary information for VRF default
Router identifier 100.0.0.180, local AS number 64513
Neighbor Status Codes: m - Under maintenance
  Neighbor    V AS           MsgRcvd   MsgSent  InQ OutQ  Up/Down State   PfxRcd PfxAcc
  100.0.0.26  4 64512             70       104    0    0 00:37:25 Estab   0      0
  100.0.0.34  4 64512             52       101    0    0 00:41:05 Estab   4      4
  100.0.0.183 4 64512             54        90    0    0 00:37:14 Estab   9      9
  100.0.0.184 4 65184           1663      1907    0    0 01:05:09 Estab   18     18
  100.0.3.41  4 64512            153       244    0    0 02:06:36 Estab   8      8
  100.0.37.9  4 64512             97       155    0    0 00:41:33 Estab   4      4
```

## show bgp evpn instance

```text
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


! IP routing not enabled
```

## show interfaces counters rates | nz

```text
Port      Name        Intvl   In Mbps      %  In Kpps  Out Mbps      % Out Kpps
Et3       PE23-J2-183  0:05       0.7   0.0%        0       0.7   0.0%        0
Et4       PE24-J2-184  0:05       2.7   0.0%        0       2.7   0.0%        0
Et8       h3c_21       0:05       0.9   0.0%        0       0.9   0.0%        0
Et9       Huawei-34    0:05       3.3   0.0%        0       3.3   0.0%        0
Et12      Ciena-3      0:05       0.9   0.0%        0       0.9   0.0%        0
Et15      rbbn-31      0:05       0.9   0.0%        0       0.9   0.0%        0
Et17      Cisco-ASR9K  0:05       0.7   0.0%        0       0.7   0.0%        0
Et49/1    Jnpr-MX304-  0:05       0.7   0.0%        0       0.7   0.0%        0
```

## show running-config section router bgp

```text
router bgp 64513
   router-id 100.0.0.180
   distance bgp 20 200 200
   bgp route-reflector preserve-attributes always
   maximum-paths 8 ecmp 16
   bgp listen range 100.0.0.0/8 peer-group EVPN-RR-CLIENTS remote-as 64512
   neighbor EVPN-RR-CLIENTS peer group
   neighbor EVPN-RR-CLIENTS remote-as 64512
   neighbor EVPN-RR-CLIENTS next-hop-unchanged
   neighbor EVPN-RR-CLIENTS update-source Loopback0
   neighbor EVPN-RR-CLIENTS ebgp-multihop 3
   neighbor EVPN-RR-CLIENTS route-reflector-client
   neighbor EVPN-RR-CLIENTS additional-paths send any
   neighbor EVPN-RR-CLIENTS send-community
   neighbor EVPN-RR-CLIENTS maximum-routes 12000
   neighbor 100.0.0.184 remote-as 65184
   neighbor 100.0.0.184 next-hop-unchanged
   neighbor 100.0.0.184 update-source Loopback0
   neighbor 100.0.0.184 ebgp-multihop 3
   neighbor 100.0.0.184 additional-paths send any
   neighbor 100.0.0.184 send-community
   !
   address-family evpn
      neighbor EVPN-RR-CLIENTS activate
      neighbor EVPN-RR-CLIENTS encapsulation mpls next-hop-self source-interface Loopback0
      neighbor 100.0.0.184 activate
      neighbor 100.0.0.184 encapsulation mpls next-hop-self source-interface Loopback0
   !
   address-family ipv4
      no neighbor EVPN-RR-CLIENTS activate
```

## show running-config section interfaces

```text
alias d show interfaces description | grep -v 'not\|down'
```

## show bgp vpn-ipv4 detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.180, local AS number 64513
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

