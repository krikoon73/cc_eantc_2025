# Test results for PE22-J2-182

## show version

```text
Arista DCS-7280SR3K-48YC8-F
Hardware version: 11.02
Serial number: JPE21115970
Hardware MAC address: 2cdd.e90b.25b7
System MAC address: 2cdd.e90b.25b7

Software image version: 4.31.2F-35053453.eostrunk.1 (engineering build)
Architecture: i686
Internal build version: 4.31.2F-35053453.eostrunk.1
Internal build ID: d771a93a-e2ca-40ce-9990-6f081af928b4
Image format version: 3.0
Image optimization: Default

Uptime: 2 days, 7 hours and 0 minutes
Total memory: 65734516 kB
Free memory: 62475580 kB

```

## show interfaces status

```text
Port       Name   Status       Vlan     Duplex Speed  Type         Flags Encapsulation
Et1               connected    routed   full   10G    10GBASE-SRL                    
Et2               notconnect   1        full   25G    Not Present                    
Et3               notconnect   1        full   25G    Not Present                    
Et4               notconnect   1        full   25G    Not Present                    
Et5               connected    in Po100 full   10G    10GBASE-SRL                    
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
Et39              notconnect   1        full   25G    Not Present                    
Et40              notconnect   1        full   25G    Not Present                    
Et41              notconnect   1        full   25G    Not Present                    
Et42              notconnect   1        full   25G    Not Present                    
Et43              notconnect   1        full   25G    Not Present                    
Et44              notconnect   1        full   25G    Not Present                    
Et45              notconnect   1        full   25G    Not Present                    
Et46              notconnect   1        full   25G    Not Present                    
Et47              connected    1        full   10G    10GBASE-SRL                    
Et48              connected    1        full   10G    10GBASE-SRL                    
Et49/1            notconnect   1        full   100G   Not Present                    
Et50/1            notconnect   1        full   100G   Not Present                    
Et51/1            notconnect   1        full   100G   Not Present                    
Et52/1            notconnect   1        full   100G   Not Present                    
Et53/1            notconnect   1        full   100G   Not Present                    
Et54/1            notconnect   1        full   100G   Not Present                    
Et55/1            notconnect   1        full   100G   Not Present                    
Et56/1            notconnect   1        full   100G   Not Present                    
Ma1               connected    routed   a-full a-1G   10/100/1000                    
Po100             connected    trunk    full   10G    N/A                            

```

## show bgp evpn summary

```text
BGP summary information for VRF default
Router identifier 100.0.0.182, local AS number 64512
Neighbor Status Codes: m - Under maintenance
  Description              Neighbor    V AS           MsgRcvd   MsgSent  InQ OutQ  Up/Down State   PfxRcd PfxAcc
  RR_ANET                  100.0.0.180 4 64512           5423      3886    0    0    1d01h Estab   118    118
  RR_Cisco                 100.0.3.58  4 64512           2379      1987    0    0 01:57:47 Estab   104    104
```

## show bgp evpn instance

```text
EVPN instance: VLAN 2181
  Route distinguisher: 100.0.0.182:2181
  Route target import: Route-Target-AS:2181:2181
  Route target export: Route-Target-AS:2181:2181
  Service interface: VLAN-based
  Local MPLS IP address: 100.0.0.182
  VXLAN: disabled
  MPLS: enabled
  Label allocation mode: per-instance
  MAC route MPLS label: 1041533
  IMET route MPLS label: 1047448
  AD route MPLS label: 1041533
  Local ethernet segment:
    ESI: 0000:0000:0000:0181:0182
      Interface: Port-Channel100
      Mode: all-active
      State: up
      ESI label: 1047648
      ES-Import RT: 00:00:18:10:01:82
      DF election algorithm: preference
      Designated forwarder: 100.0.0.182
EVPN instance: VLAN 2301
  Route distinguisher: 100.0.0.182:2301
  Route target import: Route-Target-AS:2301:2301
  Route target export: Route-Target-AS:2301:2301
  Service interface: VLAN-based
  Local MPLS IP address: 100.0.0.182
  VXLAN: disabled
  MPLS: enabled
  Label allocation mode: per-instance
  MAC route MPLS label: 1046284
  IMET route MPLS label: 1043986
  AD route MPLS label: 1046284
  Remote ethernet segment:
    ESI: 0000:0000:0000:0027:0026
    Active TEPs: 100.0.0.27
    ESI: 0000:0000:0000:0183:0184
    Active TEPs: 100.0.0.183, 100.0.0.184
    ESI: 0001:0203:0405:0607:0802
    Active TEPs: 100.0.0.34
  Local ethernet segment:
    ESI: 0000:0000:0000:0181:0182
      Interface: Port-Channel100
      Mode: all-active
      State: up
      ESI label: 1047648
      ES-Import RT: 00:00:18:10:01:82
      DF election algorithm: preference
      Designated forwarder: 100.0.0.182
EVPN instance: VLAN 2302
  Route distinguisher: 100.0.0.182:2302
  Route target import: Route-Target-AS:2302:2302
  Route target export: Route-Target-AS:2302:2302
  Service interface: VLAN-based
  Local MPLS IP address: 100.0.0.182
  VXLAN: disabled
  MPLS: enabled
  Label allocation mode: per-instance
  MAC route MPLS label: 1047390
  IMET route MPLS label: 1040999
  AD route MPLS label: 1047390
  Remote ethernet segment:
    ESI: 0000:0000:0000:0183:0184
    Active TEPs: 100.0.0.183, 100.0.0.184
  Local ethernet segment:
    ESI: 0000:0000:0000:0181:0182
      Interface: Port-Channel100
      Mode: all-active
      State: up
      ESI label: 1047648
      ES-Import RT: 00:00:18:10:01:82
      DF election algorithm: preference
      Designated forwarder: 100.0.0.182
EVPN instance: VLAN-aware bundle 2303-2304
  Route distinguisher: 100.0.0.182:2303
  Route target import: Route-Target-AS:2303:2303
  Route target export: Route-Target-AS:2303:2303
  Service interface: VLAN-aware bundle
  Local MPLS IP address: 100.0.0.182
  VXLAN: disabled
  MPLS: enabled
  Label allocation mode: per-instance
  MAC route MPLS label: 1045184
  IMET route MPLS label: 1041763
  AD route MPLS label: 1045184
  Remote ethernet segment:
    ESI: 0000:0000:0000:0027:0026
    Active TEPs: 100.0.0.27
    ESI: 0000:0000:0000:0183:0184
    Active TEPs: 100.0.0.183, 100.0.0.184
  Local ethernet segment:
    ESI: 0000:0000:0000:0181:0182
      Interface: Port-Channel100
      Mode: all-active
      State: up
      ESI label: 1047648
      ES-Import RT: 00:00:18:10:01:82
      DF election algorithm: preference
      Designated forwarder: 100.0.0.182
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

