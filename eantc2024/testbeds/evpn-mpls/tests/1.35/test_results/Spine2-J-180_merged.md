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

Uptime: 2 days, 1 hour and 9 minutes
Total memory: 8098968 kB
Free memory: 6056872 kB

```

## show interfaces status

```text
Port       Name            Status       Vlan     Duplex Speed  Type         Flags Encapsulation
Et1                        connected    routed   full   10G    10GBASE-SRL                    
Et2                        connected    routed   full   10G    10GBASE-SRL                    
Et3                        connected    routed   full   10G    10GBASE-SRL                    
Et4                        connected    routed   full   10G    10GBASE-SRL                    
Et5                        notconnect   1        full   10G    Not Present                    
Et6                        notconnect   1        full   10G    Not Present                    
Et7                        notconnect   1        full   10G    Not Present                    
Et8                        notconnect   routed   full   10G    10GBASE-SRL                    
Et9        Huawei-34       connected    routed   full   10G    10GBASE-SRL                    
Et10       H3C-18          connected    routed   full   10G    10GBASE-SRL                    
Et11                       connected    routed   full   10G    10GBASE-SRL                    
Et12       Ciena-3         connected    routed   full   10G    10GBASE-SRL                    
Et13                       notconnect   1        full   10G    Not Present                    
Et14                       notconnect   1        full   10G    Not Present                    
Et15       rbbn-31         connected    routed   full   10G    10GBASE-SRL                    
Et16                       notconnect   1        full   10G    Not Present                    
Et17       Cisco-ASR9K-341 connected    routed   full   10G    10GBASE-SRL                    
Et18       Cisco-NCS5K-345 connected    routed   full   10G    10GBASE-SRL                    
Et19       Cisco-NCS5K-48  connected    routed   full   10G    10GBASE-SRL                    
Et20       Cisco-8K-54     disabled     routed   full   10G    10GBASE-AR                     
Et21       Cisco-NCS57-45  connected    routed   full   10G    10GBASE-SRL                    
Et22                       notconnect   1        full   10G    Not Present                    
Et23       H3C-26          connected    routed   full   10G    10GBASE-SRL                    
Et24       H3C-27          connected    routed   full   10G    10GBASE-SRL                    
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
Et44                       notconnect   1        full   10G    Not Present                    
Et45                       notconnect   1        full   10G    Not Present                    
Et46                       notconnect   1        full   10G    Not Present                    
Et47                       notconnect   1        full   10G    Not Present                    
Et48                       connected    routed   full   10G    10GBASE-SRL                    
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
Router identifier 100.0.0.180, local AS number 64512
Neighbor Status Codes: m - Under maintenance
  Neighbor    V AS           MsgRcvd   MsgSent  InQ OutQ  Up/Down State   PfxRcd PfxAcc
  100.0.0.3   4 64512             74       303    0    0 01:08:23 Estab   0      0
  100.0.0.18  4 64512           1765      2317    0    0 22:17:57 Estab   1      1
  100.0.0.21  4 64512            152       443    0  644 01:59:52 Estab   0      0
  100.0.0.26  4 64512            462      1323    0    0 05:42:21 Estab   5      5
  100.0.0.27  4 64512            441      1197    0    0 05:56:34 Estab   9      9
  100.0.0.31  4 64512            288       733    0    0 01:31:13 Estab   4      4
  100.0.0.34  4 64512           2034      3115    0    0    1d03h Estab   3      3
  100.0.0.56  4 64512           5514      9279    0    0    1d20h Estab   36     36
  100.0.0.181 4 64512            224       555    0    0 02:54:25 Estab   5      5
  100.0.0.182 4 64512           1794      2897    0    0    1d01h Estab   16     16
  100.0.0.183 4 64512           3133      4609    0    0    1d20h Estab   16     16
  100.0.0.184 4 64512           3137      4603    0    0    1d20h Estab   16     16
  100.0.3.45  4 64512           1349      2321    0    0 22:17:31 Estab   12     12
  100.0.3.48  4 64512           1349      2327    0    0 22:17:41 Estab   10     10
  100.0.30.9  4 64512           3107      5171    0    0 22:17:57 Estab   1      1
  100.0.31.4  4 64512             47       268    0    0 00:19:54 Estab   0      0
```

## show bgp evpn instance

```text
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

