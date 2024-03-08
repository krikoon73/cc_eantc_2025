# Test results for PE42-J2-162

## show version

```text
Arista DCS-7280SR3-40YC6-F
Hardware version: 11.02
Serial number: JPA2339P1QH
Hardware MAC address: 606b.5b2e.f3fd
System MAC address: 606b.5b2e.f3fd

Software image version: 4.31.2F
Architecture: i686
Internal build version: 4.31.2F-35442146.4312F
Internal build ID: 635a071a-386e-447f-942c-bcc34d9ffd3c
Image format version: 3.0
Image optimization: Default

Uptime: 4 hours and 49 minutes
Total memory: 8099732 kB
Free memory: 5669916 kB

```

## show interfaces status

```text
Port       Name     Status       Vlan     Duplex Speed  Type         Flags Encapsulation
Et1                 notconnect   1        full   25G    Not Present                    
Et2                 notconnect   1        full   25G    Not Present                    
Et3                 notconnect   1        full   25G    Not Present                    
Et4                 notconnect   1        full   25G    Not Present                    
Et5                 notconnect   1        full   10G    10GBASE-SRL                    
Et6                 notconnect   1        full   25G    Not Present                    
Et7                 notconnect   1        full   25G    Not Present                    
Et8                 notconnect   1        full   25G    Not Present                    
Et9                 notconnect   1        full   25G    Not Present                    
Et10                disabled     routed   full   10G    10GBASE-SRL                    
Et11                notconnect   1        full   25G    Not Present                    
Et12                disabled     trunk    full   10G    10GBASE-LR                     
Et13                notconnect   1        full   25G    Not Present                    
Et14                notconnect   1        full   25G    Not Present                    
Et15                notconnect   1        full   25G    Not Present                    
Et16                notconnect   1        full   25G    Not Present                    
Et17                notconnect   1        full   25G    Not Present                    
Et18                notconnect   1        full   25G    Not Present                    
Et19                notconnect   1        full   25G    Not Present                    
Et20                disabled     routed   full   10G    10GBASE-SR                     
Et21                notconnect   1        full   25G    Not Present                    
Et22                notconnect   1        full   25G    Not Present                    
Et23                notconnect   1        full   25G    Not Present                    
Et24                notconnect   1        full   25G    Not Present                    
Et25                notconnect   1        full   25G    Not Present                    
Et26                notconnect   1        full   25G    Not Present                    
Et27                notconnect   1        full   25G    Not Present                    
Et28                notconnect   1        full   25G    Not Present                    
Et29                notconnect   1        full   25G    Not Present                    
Et30                notconnect   1        full   25G    Not Present                    
Et31                notconnect   1        full   25G    Not Present                    
Et32                notconnect   1        full   25G    Not Present                    
Et33                notconnect   1        full   25G    Not Present                    
Et34                notconnect   1        full   25G    Not Present                    
Et35                notconnect   1        full   25G    Not Present                    
Et36                notconnect   1        full   25G    Not Present                    
Et37                errdisabled  1        full   25G    Not Present                    
Et38                errdisabled  1        full   25G    Not Present                    
Et39                disabled     1        full   10G    10GBASE-SRL                    
Et40                disabled     1        full   10G    10GBASE-SRL                    
Et41/1     Nokia_57 connected    routed   full   10G    40GBASE-SR4                    
Et41/2              notconnect   1        full   10G    40GBASE-SR4                    
Et41/3              notconnect   1        full   10G    40GBASE-SR4                    
Et41/4              notconnect   1        full   10G    40GBASE-SR4                    
Et43/1              notconnect   1        full   100G   Not Present                    
Et44/1              notconnect   1        full   100G   Not Present                    
Et45/1              notconnect   1        full   100G   Not Present                    
Et46/1              notconnect   1        full   100G   Not Present                    
Ma1                 connected    routed   a-full a-1G   10/100/1000                    

```

## show lldp neighbors

```text
Last table change time   : 4:44:54 ago
Number of table inserts  : 2
Number of table deletes  : 0
Number of table drops    : 0
Number of table age-outs : 0

Port            Neighbor Device ID       Neighbor Port ID    TTL
------------ ------------------------ ---------------------- ---
Et41/1          NOKIA-SR2-57             1610899526          121
Ma1             extreme-x460-1           22                  120

```

## show isis segment-routing prefix-segments

```text

System ID: anet-PE42-J2-162			Instance: 'IPV6'
SR supported Data-plane: MPLS			SR Router ID: 100.0.0.162

Node: 11     Proxy-Node: 0      Prefix: 0       Total Segments: 11

Flag Descriptions: R: Re-advertised, N: Node Segment, P: no-PHP
                   E: Explicit-NULL, V: Value, L: Local
Segment status codes: * - Self originated Prefix, L1 - level 1, L2 - level 2, ! - SR-unreachable,
                      # - Some IS-IS next-hops are SR-unreachable
   Prefix                      SID Type       Flags                        System ID       Level Protection  Algorithm   
   ------------------------- ----- ---------- ---------------------------- --------------- ----- ----------- -------------
   10.0.0.57/32                 57 Node       R:0 N:1 P:1 E:0 V:0 L:0      NOKIA-SR2-57    L2    unprotected SPF         
   10.0.0.59/32                 59 Node       R:0 N:1 P:1 E:0 V:0 L:0      Nokia-59-IXRe2  L2    unprotected SPF         
   2002::57/128                157 Node       R:0 N:1 P:1 E:0 V:0 L:0      NOKIA-SR2-57    L2    node        SPF         
   2002::57/128                728 Node       R:0 N:1 P:1 E:0 V:0 L:0      NOKIA-SR2-57    L2    unprotected 128         
   2002::59/128                159 Node       R:0 N:1 P:1 E:0 V:0 L:0      Nokia-59-IXRe2  L2    node        SPF         
   2002::59/128                928 Node       R:0 N:1 P:1 E:0 V:0 L:0      Nokia-59-IXRe2  L2    unprotected 128         
*  2002::162/128              1162 Node       R:0 N:1 P:0 E:0 V:0 L:0      anet-PE42-J2-162 L2    unprotected SPF         
   2002::303/128               303 Node       R:0 N:1 P:0 E:0 V:0 L:0      juniper_303_mx204 L2    node        SPF         
   2002::303/128              1103 Node       R:0 N:1 P:0 E:0 V:0 L:0      juniper_303_mx204 L2    unprotected 128         
   2002::304/128               304 Node       R:0 N:1 P:0 E:0 V:0 L:0      juniper_304_mx204 L2    node        SPF         
   2002::304/128              1104 Node       R:0 N:1 P:0 E:0 V:0 L:0      juniper_304_mx204 L2    unprotected 128         
```

## show isis neighbors

```text
 
Instance  VRF      System Id        Type Interface          SNPA              State Hold time   Circuit Id          
IPV6      default  NOKIA-SR2-57     L2   Ethernet41/1       P2P               UP    23          00                  
```

## show ipv6 bgp summary

```text
BGP summary information for VRF default
Router identifier 100.0.0.162, local AS number 65000
Neighbor Status Codes: m - Under maintenance
  Neighbor V AS           MsgRcvd   MsgSent  InQ OutQ  Up/Down State   PfxRcd PfxAcc
```

## show bgp evpn summary

```text
BGP summary information for VRF default
Router identifier 100.0.0.162, local AS number 65000
Neighbor Status Codes: m - Under maintenance
  Neighbor  V AS           MsgRcvd   MsgSent  InQ OutQ  Up/Down State   PfxRcd PfxAcc
  2002::59  4 65000            674      3341    0    0 01:38:58 Estab   2      2
  2002::304 4 65000          41110     41362    0    0 00:00:00 Estab(NotNegotiated)
```

## show bgp vpn-ipv4 summary

```text
BGP summary information for VRF default
Router identifier 100.0.0.162, local AS number 65000
Neighbor Status Codes: m - Under maintenance
  Neighbor  V AS           MsgRcvd   MsgSent  InQ OutQ  Up/Down State   PfxRcd PfxAcc
  2002::59  4 65000            674      3341    0    0 01:38:58 Estab   3      3
  2002::304 4 65000          41110     41362    0    0 00:00:00 Estab   0      0
```

## show bgp vpn-ipv6 summary

```text
BGP summary information for VRF default
Router identifier 100.0.0.162, local AS number 65000
Neighbor Status Codes: m - Under maintenance
  Neighbor  V AS           MsgRcvd   MsgSent  InQ OutQ  Up/Down State   PfxRcd PfxAcc
  2002::59  4 65000            674      3341    0    0 01:38:58 Estab   6      6
  2002::304 4 65000          41110     41362    0    0 00:00:00 Estab   0      0
```

