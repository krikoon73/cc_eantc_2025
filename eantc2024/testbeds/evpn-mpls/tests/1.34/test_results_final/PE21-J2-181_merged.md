# Test results for PE21-J2-181

## show version

```text
Arista DCS-7280SR3K-48YC8-F
Hardware version: 11.02
Serial number: JPE21116007
Hardware MAC address: 2cdd.e90b.2283
System MAC address: 2cdd.e90b.2283

Software image version: 4.29.2F
Architecture: i686
Internal build version: 4.29.2F-30640700.4292F
Internal build ID: d65c8013-3e2b-4be9-ad9e-652efbbce887
Image format version: 3.0
Image optimization: Default

Uptime: 21 hours and 47 minutes
Total memory: 65841228 kB
Free memory: 62373512 kB

```

## show interfaces status

```text
! * Incomplete encapsulation information. Use 'show interface encapsulation vlan' instead
Port       Name   Status       Vlan     Duplex Speed  Type         Flags Encapsulation
Et1               connected    routed   full   10G    10GBASE-SRL                    
Et2               notconnect   1        full   25G    Not Present                    
Et3               notconnect   1        full   25G    Not Present                    
Et4               notconnect   1        full   25G    Not Present                    
Et5               notconnect   routed   full   10G    10GBASE-SRL                    
Et5.2311          notconnect   routed   full   10G    subinterface       *           
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
Po100             notconnect   trunk    full   unconf N/A                            

```

## show bgp evpn summary

```text
BGP summary information for VRF default
Router identifier 100.0.0.181, local AS number 64512
Neighbor Status Codes: m - Under maintenance
  Neighbor    V AS           MsgRcvd   MsgSent  InQ OutQ  Up/Down State   PfxRcd PfxAcc
  100.0.0.180 4 64512           1035       480    0    0 02:54:24 Estab   129    129
  100.0.3.58  4 64512            883       488    0    0 01:57:37 Estab   115    115
```

## show bgp evpn instance

```text
EVPN instance: VLAN 2181
  Route distinguisher: 100.0.0.181:2181
  Route target import: Route-Target-AS:2181:2181
  Route target export: Route-Target-AS:2181:2181
  Service interface: VLAN-based
  Local MPLS IP address: 100.0.0.181
  VXLAN: disabled
  MPLS: enabled
  Label allocation mode: per-instance
  MAC route MPLS label: 1047390
  IMET route MPLS label: 1040999
  AD route MPLS label: 1047390
  Local ethernet segment:
    ESI: 0000:0000:0000:0181:0182
      Interface: Port-Channel100
      Mode: all-active
      State: down
      ESI label: 1036288
      ES-Import RT: 00:00:18:10:01:82
      DF election state: pending
      Designated forwarder: 
EVPN instance: VLAN 2301
  Route distinguisher: 100.0.0.181:2301
  Route target import: Route-Target-AS:2301:2301
  Route target export: Route-Target-AS:2301:2301
  Service interface: VLAN-based
  Local MPLS IP address: 100.0.0.181
  VXLAN: disabled
  MPLS: enabled
  Label allocation mode: per-instance
  MAC route MPLS label: 1045184
  IMET route MPLS label: 1041763
  AD route MPLS label: 1045184
  Local ethernet segment:
    ESI: 0000:0000:0000:0181:0182
      Interface: Port-Channel100
      Mode: all-active
      State: down
      ESI label: 1036288
      ES-Import RT: 00:00:18:10:01:82
      DF election state: pending
      Designated forwarder: 
EVPN instance: VLAN 2302
  Route distinguisher: 100.0.0.181:2302
  Route target import: Route-Target-AS:2302:2302
  Route target export: Route-Target-AS:2302:2302
  Service interface: VLAN-based
  Local MPLS IP address: 100.0.0.181
  VXLAN: disabled
  MPLS: enabled
  Label allocation mode: per-instance
  MAC route MPLS label: 1042318
  IMET route MPLS label: 1036782
  AD route MPLS label: 1042318
  Local ethernet segment:
    ESI: 0000:0000:0000:0181:0182
      Interface: Port-Channel100
      Mode: all-active
      State: down
      ESI label: 1036288
      ES-Import RT: 00:00:18:10:01:82
      DF election state: pending
      Designated forwarder: 
EVPN instance: VLAN-aware bundle 2303-2304
  Route distinguisher: 100.0.0.181:2303
  Route target import: Route-Target-AS:2303:2303
  Route target export: Route-Target-AS:2303:2303
  Service interface: VLAN-aware bundle
  Local MPLS IP address: 100.0.0.181
  VXLAN: disabled
  MPLS: enabled
  Label allocation mode: per-instance
  MAC route MPLS label: 1046284
  IMET route MPLS label: 1043986
  AD route MPLS label: 1046284
  Local ethernet segment:
    ESI: 0000:0000:0000:0181:0182
      Interface: Port-Channel100
      Mode: all-active
      State: down
      ESI label: 1036288
      ES-Import RT: 00:00:18:10:01:82
      DF election state: pending
      Designated forwarder: 
EVPN instance: VPWS 2311
  Route distinguisher: 100.0.0.181:2310
  Route target import: Route-Target-AS:2310:2310
  Route target export: Route-Target-AS:2310:2310
  Service interface: VLAN-based
  Local MPLS IP address: 100.0.0.181
  VXLAN: disabled
  MPLS: enabled
  Label allocation mode: per-pseudowire
  L2 MTU: ignored
  Control word: disabled
  Pseudowires:
    Pseudowire pw1
      Status: down (no request)
      Local VPWS ID: 2310
      Remote VPWS ID: 2311
```

## show patch panel detail

```text
PW Fault Legend:
   ET-IN - Ethernet receive fault
   ET-OUT - Ethernet transmit fault
   TUN-IN - Tunnel receive fault
   TUN-OUT - Tunnel transmit fault
   NF - Pseudowire not forwarding (other reason)

Patch: 2311, Status: Down, Last change: 2:16:13 ago
   Connector 1: Ethernet5.2311
      Status: Interface mode
   Connector 2: BGP VPWS 2311 Pseudowire pw1
      Status: Interface unavailable
      Local MPLS label: 100000
      EVPN VPWS type: VLAN-based
      Flow label used: no
```

