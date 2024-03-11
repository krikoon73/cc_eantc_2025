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

Uptime: 2 days, 7 hours and 0 minutes
Total memory: 8147100 kB
Free memory: 5774784 kB

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
  Description              Neighbor    V AS           MsgRcvd   MsgSent  InQ OutQ  Up/Down State   PfxRcd PfxAcc
  RR_ANET                  100.0.0.180 4 64512           5362      3922    0    0    1d20h Estab   118    118
  RR_Cisco                 100.0.3.58  4 64512           2304      1963    0    0 01:57:33 Estab   104    104
```

## show bgp evpn instance

```text
EVPN instance: VLAN 2183
  Route distinguisher: 100.0.0.184:2183
  Route target import: Route-Target-AS:2183:2183
  Route target export: Route-Target-AS:2183:2183
  Service interface: VLAN-based
  Local MPLS IP address: 100.0.0.184
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
      State: up
      ESI label: 1036288
      ES-Import RT: 00:00:18:30:01:84
      DF election algorithm: preference
      Designated forwarder: 100.0.0.183
      Non-Designated forwarder: 100.0.0.184
EVPN instance: VLAN 2301
  Route distinguisher: 100.0.0.184:2301
  Route target import: Route-Target-AS:2301:2301
  Route target export: Route-Target-AS:2301:2301
  Service interface: VLAN-based
  Local MPLS IP address: 100.0.0.184
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
      State: up
      ESI label: 1036288
      ES-Import RT: 00:00:18:30:01:84
      DF election algorithm: preference
      Designated forwarder: 100.0.0.183
      Non-Designated forwarder: 100.0.0.184
EVPN instance: VLAN 2302
  Route distinguisher: 100.0.0.184:2302
  Route target import: Route-Target-AS:2302:2302
  Route target export: Route-Target-AS:2302:2302
  Service interface: VLAN-based
  Local MPLS IP address: 100.0.0.184
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
      State: up
      ESI label: 1036288
      ES-Import RT: 00:00:18:30:01:84
      DF election algorithm: preference
      Designated forwarder: 100.0.0.183
      Non-Designated forwarder: 100.0.0.184
EVPN instance: VLAN-aware bundle 2303-2304
  Route distinguisher: 100.0.0.184:2303
  Route target import: Route-Target-AS:2303:2303
  Route target export: Route-Target-AS:2303:2303
  Service interface: VLAN-aware bundle
  Local MPLS IP address: 100.0.0.184
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
      State: up
      ESI label: 1036288
      ES-Import RT: 00:00:18:30:01:84
      DF election algorithm: preference
      Designated forwarder: 100.0.0.183
      Non-Designated forwarder: 100.0.0.184
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

