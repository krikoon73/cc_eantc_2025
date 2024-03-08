# Test results for Harness1-J-205

## show version

```text
Arista DCS-7280SR-48C6-F
Hardware version: 01.02
Serial number: JPE16200911
Hardware MAC address: 444c.a873.a0ad
System MAC address: 444c.a873.a0ad

Software image version: 4.28.2F
Architecture: i686
Internal build version: 4.28.2F-28369039.4282F
Internal build ID: 9b26a848-014e-4308-a976-9888833fc462
Image format version: 3.0
Image optimization: Sand-4GB

Uptime: 2 days, 20 hours and 50 minutes
Total memory: 8098932 kB
Free memory: 5990600 kB

```

## show interfaces status

```text
Port       Name         Status       Vlan     Duplex Speed  Type         Flags Encapsulation
Et1        ANET-201     connected    in Po100 full   10G    10GBASE-SRL                    
Et2        ANET-202     connected    in Po100 full   10G    10GBASE-SRL                    
Et3        ANET-203     connected    in Po200 full   10G    10GBASE-SRL                    
Et4        ANET-204     connected    in Po200 full   10G    10GBASE-SRL                    
Et5        ANET-206     connected    1        a-full a-10G  10GBASE-T                      
Et6                     notconnect   1        full   10G    Not Present                    
Et7                     notconnect   1        full   10G    Not Present                    
Et8                     notconnect   1        full   10G    Not Present                    
Et9                     notconnect   1        full   10G    Not Present                    
Et10                    notconnect   1        full   10G    Not Present                    
Et11                    notconnect   1        full   10G    Not Present                    
Et12                    notconnect   1        full   10G    Not Present                    
Et13       Cisco-45-46  connected    in Po301 full   10G    10GBASE-AR                     
Et14       Cisco-45-46  connected    in Po301 full   10G    10GBASE-AR                     
Et15                    connected    trunk    full   10G    10GBASE-AR                     
Et16                    connected    trunk    full   10G    10GBASE-AR                     
Et17                    connected    1        full   10G    10GBASE-AR                     
Et18                    notconnect   1        full   10G    Not Present                    
Et19                    notconnect   1        full   10G    Not Present                    
Et20                    notconnect   1        full   10G    Not Present                    
Et21       Nokia-56     connected    trunk    full   10G    10GBASE-SRL                    
Et22                    notconnect   1        full   10G    Not Present                    
Et23                    notconnect   1        full   10G    Not Present                    
Et24                    notconnect   1        full   10G    Not Present                    
Et25       Keysight-Gen connected    trunk    full   10G    10GBASE-SRL                    
Et26                    notconnect   1        full   10G    Not Present                    
Et27                    connected    in Po300 full   10G    10GBASE-SRL                    
Et28                    notconnect   in Po300 full   10G    10GBASE-SRL                    
Et29                    notconnect   1        full   10G    Not Present                    
Et30                    notconnect   1        full   10G    Not Present                    
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
Et49/1                  disabled     1        full   100G   Not Present                    
Et50/1                  notconnect   1        full   100G   Not Present                    
Et51/1                  notconnect   1        full   100G   Not Present                    
Et52/1                  notconnect   1        full   100G   Not Present                    
Et53/1                  disabled     1        full   100G   Not Present                    
Et54/1                  disabled     1        full   100G   Not Present                    
Ma1                     connected    routed   a-full a-1G   10/100/1000                    
Po100                   connected    trunk    full   20G    N/A                            
Po200                   connected    trunk    full   20G    N/A                            
Po300                   connected    trunk    full   10G    N/A                            
Po301                   connected    trunk    full   20G    N/A                            
Po302                   notconnect   1        full   unconf N/A                            

```

## show lldp neighbors

```text
Last table change time   : 17:56:33 ago
Number of table inserts  : 46
Number of table deletes  : 32
Number of table drops    : 0
Number of table age-outs : 0

Port          Neighbor Device ID              Neighbor Port ID        TTL
---------- ------------------------------- -------------------------- ---
Et1           PE11-JP-201.ns.eantc.de         Ethernet5               120
Et2           PE12-JP-202.ns.eantc.de         Ethernet5               120
Et3           PE13-T3-203.ns.eantc.de         Ethernet5               120
Et4           PE14-T3-204.ns.eantc.de         Ethernet5               120
Et5           P15-T3-206.eantc.de             Ethernet5               120
Et13          Cisco_45_N9K-C93240YC-FX2       Ethernet1/5             120
Et14          Cisco_46_N9K-C93240YC-FX2       Ethernet1/5             120
Et15          Cisco_40_N9K-C93180YC-FX3       Ethernet1/5             120
Et16          Cisco_42_N9K-C93400LD-H1        Ethernet1/5             120
Et17          Cisco_44_N3K-C36180YC-R         Ethernet1/5             120
Et21          185b.0089.c3cc                  1610899587              121
Et27          h3c_22_S6850-56HF               Twenty-FiveGigE1/0/4    121
Et48          SPINE1-J-200.ns.eantc.de        Ethernet48              120
Ma1           extreme-x460-1                  24                      120

```

