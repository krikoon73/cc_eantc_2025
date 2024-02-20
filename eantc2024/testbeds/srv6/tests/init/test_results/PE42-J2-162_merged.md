# Test results for PE42-J2-162

## show version

```text
Arista DCS-7280SR3-40YC6-F
Hardware version: 11.02
Serial number: JPA2339P1QH
Hardware MAC address: 606b.5b2e.f3fd
System MAC address: 606b.5b2e.f3fd

Software image version: 4.31.0F-34472350.binoshmonsrv6ImgCDD43101 (engineering build)
Architecture: x86_64
Internal build version: 4.31.0F-34472350.binoshmonsrv6ImgCDD43101
Internal build ID: 6aa1c3ff-36f3-4f04-af26-9fc35d05e1eb
Image format version: 3.0
Image optimization: Default

Uptime: 17 hours and 43 minutes
Total memory: 8099732 kB
Free memory: 5169396 kB

```

## show interfaces status

```text
Port       Name   Status       Vlan     Duplex Speed  Type         Flags Encapsulation
Et1               notconnect   1        full   25G    Not Present                    
Et2               notconnect   1        full   25G    Not Present                    
Et3               notconnect   1        full   25G    Not Present                    
Et4               notconnect   1        full   25G    Not Present                    
Et5               notconnect   1        full   10G    10GBASE-SRL                    
Et6               notconnect   1        full   25G    Not Present                    
Et7               notconnect   1        full   25G    Not Present                    
Et8               notconnect   1        full   25G    Not Present                    
Et9               notconnect   1        full   25G    Not Present                    
Et10              connected    routed   full   10G    10GBASE-SRL                    
Et11              notconnect   1        full   25G    Not Present                    
Et12              connected    1        full   10G    10GBASE-LR                     
Et13              notconnect   1        full   25G    Not Present                    
Et14              notconnect   1        full   25G    Not Present                    
Et15              notconnect   1        full   25G    Not Present                    
Et16              notconnect   1        full   25G    Not Present                    
Et17              notconnect   1        full   25G    Not Present                    
Et18              notconnect   1        full   25G    Not Present                    
Et19              notconnect   1        full   25G    Not Present                    
Et20              connected    routed   full   10G    10GBASE-SR                     
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
Et37              errdisabled  1        full   25G    Not Present                    
Et38              errdisabled  1        full   25G    Not Present                    
Et39              connected    1        full   10G    10GBASE-SRL                    
Et40              connected    1        full   10G    10GBASE-SRL                    
Et41/1            notconnect   1        full   100G   Not Present                    
Et42/1            notconnect   1        full   100G   Not Present                    
Et43/1            notconnect   1        full   100G   Not Present                    
Et44/1            notconnect   1        full   100G   Not Present                    
Et45/1            notconnect   1        full   100G   Not Present                    
Et46/1            notconnect   1        full   100G   Not Present                    
Ma1               connected    routed   a-full a-1G   10/100/1000                    

```

## show lldp neighbors

```text
Last table change time   : 1:14:29 ago
Number of table inserts  : 7
Number of table deletes  : 1
Number of table drops    : 0
Number of table age-outs : 0

Port          Neighbor Device ID            Neighbor Port ID    TTL
---------- ----------------------------- ---------------------- ---
Et10          JNPR-302-MX204                564                 120
Et12          JNPR-398-QFX5120              548                 120
Et20          h344-N57B1                    TenGigE0/0/0/0/0    120
Et39          PE41-J2-161.ns.eantc.de       Ethernet39          120
Et40          PE41-J2-161.ns.eantc.de       Ethernet40          120
Ma1           extreme-x460-1                22                  120

```

## show isis neighbors

```text
 
Instance  VRF      System Id        Type Interface          SNPA              State Hold time   Circuit Id          
srv6      default  JNPR-302-MX204   L1   Ethernet10         P2P               UP    23          01                  
srv6      default  h344-N57B1       L1   Ethernet20         P2P               UP    26          00                  
```

## show segment-routing ipv6 locator

```text
SRv6 configuration for VRF default
Administrative status: enabled
Operational status: enabled
Encapsulation source address: 2002::162
Number of configured locators: 1

Locator node162
State: active
Type: classic
Prefix: fcbb:0:162::/48
IGP algorithm: SPF
Block length: 32
Function length: 16
Function allocator: classic::node162
SID function value pools: default
```

## show segment-routing ipv6 locator std

```text
SRv6 configuration for VRF default
Administrative status: enabled
Operational status: enabled
Encapsulation source address: 2002::162
Number of configured locators: 1
```

## show segment-routing ipv6 sid function allocators

```text
SRv6 SID function allocators for VRF default

Allocator classic::node162
Function length: 16
Locator users: node162
Start   End  Size Usage     
----- ----- ----- ----------
    1  1023  1023 static    
 1024 65535 64512 unassigned

```

## show segment-routing ipv6 capabilities

```text
```

## show segment-routing ipv6 route

```text
VRF default
Source Codes: B3 - BGP L3 VPN, S - Static
End Behaviors: End - Endpoint
               End.DT4 (6) - Endpoint with decapsulation and specific IPv4 (6) table lookup

```

## show bgp evpn summary

```text
BGP summary information for VRF default
Router identifier 100.0.0.162, local AS number 1
Neighbor Status Codes: m - Under maintenance
  Neighbor  V AS           MsgRcvd   MsgSent  InQ OutQ  Up/Down State   PfxRcd PfxAcc
  2002::353 4 1                 39        45    0    0 00:36:57 Estab   0      0
```

## show bgp evpn route-type ip-prefix ipv4 detail

```text
BGP routing table information for VRF default
Router identifier 100.0.0.162, local AS number 1
```

## show tunnel fib

```text
```

