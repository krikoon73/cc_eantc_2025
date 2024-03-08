# Test results for Spine1-J-200

## show version

```text
Arista DCS-7280SR-48C6-F
Hardware version: 01.00
Serial number: JPE16174588
Hardware MAC address: 444c.a873.5c75
System MAC address: 444c.a873.5c75

Software image version: 4.31.2F
Architecture: i686
Internal build version: 4.31.2F-35442146.4312F
Internal build ID: 635a071a-386e-447f-942c-bcc34d9ffd3c
Image format version: 3.0
Image optimization: Sand-4GB

Uptime: 5 hours and 4 minutes
Total memory: 8051592 kB
Free memory: 5751128 kB

```

## show interfaces status

```text
Port       Name         Status       Vlan     Duplex Speed  Type         Flags Encapsulation
Et1        A-PE11-201   connected    routed   full   10G    10GBASE-SRL                    
Et2        A-PE12-202   notconnect   routed   full   10G    10GBASE-SRL                    
Et3        A-PE13-203   connected    routed   full   10G    10GBASE-SRL                    
Et4        A-PE14-204   connected    routed   full   10G    10GBASE-SRL                    
Et5        A-PE16-206   notconnect   routed   full   10G    10GBASE-LR                     
Et6                     notconnect   1        full   10G    Not Present                    
Et7                     notconnect   1        full   10G    Not Present                    
Et8                     notconnect   1        full   10G    Not Present                    
Et9                     notconnect   1        full   10G    Not Present                    
Et10                    notconnect   1        full   10G    Not Present                    
Et11       Nokia-56     connected    routed   full   10G    10GBASE-SRL                    
Et12       Keysight-103 connected    routed   full   10G    10GBASE-SRL                    
Et13       Cisco-45-N9K disabled     routed   full   10G    10GBASE-AR                     
Et14       Cisco-46-N9K disabled     routed   full   10G    10GBASE-AR                     
Et15       Cisco-40-N9K connected    routed   full   10G    10GBASE-AR                     
Et16       Cisco-42-N9K connected    routed   full   10G    10GBASE-AR                     
Et17                    notconnect   routed   full   10G    Not Present                    
Et18                    notconnect   1        full   10G    Not Present                    
Et19                    notconnect   1        full   10G    Not Present                    
Et20                    notconnect   1        full   10G    Not Present                    
Et21                    disabled     1        full   10G    Not Present                    
Et22                    disabled     1        full   10G    Not Present                    
Et23                    disabled     1        full   10G    Not Present                    
Et24                    connected    1        full   10G    10GBASE-SR                     
Et25       H3C-23       notconnect   routed   full   10G    10GBASE-SRL                    
Et26       H3C-22       connected    routed   full   10G    10GBASE-SRL                    
Et27                    disabled     1        full   10G    Not Present                    
Et28                    disabled     1        full   10G    Not Present                    
Et29                    disabled     1        full   10G    Not Present                    
Et30                    disabled     1        full   10G    Not Present                    
Et31                    disabled     1        full   10G    Not Present                    
Et32                    disabled     1        full   10G    Not Present                    
Et33                    disabled     1        full   10G    Not Present                    
Et34                    disabled     1        full   10G    Not Present                    
Et35                    disabled     1        full   10G    Not Present                    
Et36                    disabled     1        full   10G    Not Present                    
Et37                    disabled     1        full   10G    Not Present                    
Et38                    disabled     1        full   10G    Not Present                    
Et39                    disabled     1        full   10G    Not Present                    
Et40                    disabled     1        full   10G    Not Present                    
Et41                    disabled     1        full   10G    Not Present                    
Et42                    disabled     1        full   10G    Not Present                    
Et43                    disabled     1        full   10G    Not Present                    
Et44                    disabled     1        full   10G    Not Present                    
Et45                    disabled     1        full   10G    Not Present                    
Et46                    disabled     1        full   10G    Not Present                    
Et47                    disabled     1        full   10G    Not Present                    
Et48       Spine-host   connected    trunk    full   10G    10GBASE-SRL                    
Et49/1                  disabled     routed   full   100G   Not Present                    
Et50/1                  disabled     1        full   100G   Not Present                    
Et51/1                  notconnect   routed   full   100G   Not Present                    
Et52/1                  notconnect   1        full   100G   Not Present                    
Et53/1                  disabled     1        full   100G   Not Present                    
Et54/1                  disabled     1        full   100G   Not Present                    
Ma1                     connected    routed   a-full a-1G   10/100/1000                    

```

## show lldp neighbors

```text
Last table change time   : 0:04:29 ago
Number of table inserts  : 16
Number of table deletes  : 6
Number of table drops    : 0
Number of table age-outs : 0

Port          Neighbor Device ID               Neighbor Port ID        TTL
---------- -------------------------------- -------------------------- ---
Et1           PE21-J2-181.ns.eantc.de          Ethernet1               120
Et3           PE13-T3-203.ns.eantc.de          Ethernet1               120
Et4           PE14-T3-204.ns.eantc.de          Ethernet1               120
Et11          185b.0089.c3cc                   1610899585              121
Et15          Cisco_40_N9K-C93180YC-FX3        Ethernet1/1             120
Et16          Cisco_42_N9K-C93400LD-H1         Ethernet1/1             120
Et24          juniper-314-ACX7509              et-2/0/3                120
Et26          h3c_22_S6850-56HF                Twenty-FiveGigE1/0/3    121
Et48          Harness1-J-205.ns.eantc.de       Ethernet48              120
Ma1           extreme-x460-1                   43                      120

```

