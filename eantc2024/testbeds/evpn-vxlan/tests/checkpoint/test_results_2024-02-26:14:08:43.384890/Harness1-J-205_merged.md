# Test results for Harness1-J-205

## show version

```text
Arista DCS-7280SR-48C6-F
Hardware version: 01.02
Serial number: JPE16200911
Hardware MAC address: 444c.a873.a0ad
System MAC address: 444c.a873.a0ad

Software image version: 4.31.2F
Architecture: x86_64
Internal build version: 4.31.2F-35442176.4312F
Internal build ID: 500c58e3-5beb-4481-afe9-8ad77245cc44
Image format version: 3.0
Image optimization: Sand-4GB

Uptime: 7 hours and 14 minutes
Total memory: 8051592 kB
Free memory: 5327940 kB

```

## show interfaces status

```text
! * Incomplete encapsulation information. Use 'show interface encapsulation vlan' instead
Port       Name           Status       Vlan     Duplex Speed  Type         Flags Encapsulation
Et1        ANET-201       disabled     in Po100 full   10G    10GBASE-SRL                    
Et2        ANET-202       disabled     in Po100 full   10G    10GBASE-SRL                    
Et3        ANET-203       connected    in Po200 full   10G    10GBASE-SRL                    
Et4        ANET-204       disabled     in Po200 full   10G    10GBASE-SRL                    
Et5        ANET-206       notconnect   1        auto   auto   10GBASE-T                      
Et6                       notconnect   routed   full   10G    Not Present                    
Et6.201                   notconnect   routed   full   10G    subinterface       *           
Et7                       notconnect   1        full   10G    Not Present                    
Et8                       notconnect   1        full   10G    Not Present                    
Et9                       notconnect   1        full   10G    Not Present                    
Et10                      notconnect   1        full   10G    Not Present                    
Et11                      notconnect   1        full   10G    Not Present                    
Et12                      notconnect   1        full   10G    Not Present                    
Et13       Cisco-45-46    connected    in Po301 full   10G    10GBASE-AR                     
Et14       Cisco-45-46    connected    in Po301 full   10G    10GBASE-AR                     
Et15                      connected    trunk    full   10G    10GBASE-AR                     
Et16                      connected    trunk    full   10G    10GBASE-AR                     
Et17                      connected    1        full   10G    10GBASE-AR                     
Et18                      notconnect   1        full   10G    Not Present                    
Et19                      notconnect   1        full   10G    Not Present                    
Et20                      notconnect   1        full   10G    Not Present                    
Et21       Nokia-56       connected    in Po200 full   10G    10GBASE-SRL                    
Et22                      notconnect   1        full   10G    Not Present                    
Et23                      notconnect   1        full   10G    Not Present                    
Et24                      notconnect   1        full   10G    Not Present                    
Et25       Keysight-Gen   connected    trunk    full   10G    10GBASE-SRL                    
Et26       KeySight Test  connected    routed   full   10G    10GBASE-SRL                    
Et26.201                  notconnect   routed   full   10G    subinterface       *           
Et27                      notconnect   in Po300 full   10G    10GBASE-SRL                    
Et28                      notconnect   in Po300 full   10G    10GBASE-SRL                    
Et29                      notconnect   1        full   10G    Not Present                    
Et30                      notconnect   1        full   10G    Not Present                    
Et31                      disabled     1        full   10G    Not Present                    
Et32                      disabled     1        full   10G    Not Present                    
Et33                      disabled     1        full   10G    Not Present                    
Et34                      disabled     1        full   10G    Not Present                    
Et35                      disabled     1        full   10G    Not Present                    
Et36                      disabled     1        full   10G    Not Present                    
Et37                      disabled     1        full   10G    Not Present                    
Et38                      disabled     1        full   10G    Not Present                    
Et39                      disabled     1        full   10G    Not Present                    
Et40                      disabled     1        full   10G    Not Present                    
Et41                      disabled     1        full   10G    Not Present                    
Et42                      disabled     1        full   10G    Not Present                    
Et43                      disabled     1        full   10G    Not Present                    
Et44                      disabled     1        full   10G    Not Present                    
Et45                      disabled     1        full   10G    Not Present                    
Et46                      disabled     1        full   10G    Not Present                    
Et47                      disabled     1        full   10G    Not Present                    
Et48       Spine-host     connected    trunk    full   10G    10GBASE-SRL                    
Et49/1     Nokia-GW WAN   connected    routed   full   10G    40GBASE-SR4                    
Et49/2     JNPR314-GW WAN connected    routed   full   10G    40GBASE-SR4                    
Et49/3                    notconnect   1        full   10G    40GBASE-SR4                    
Et49/4                    notconnect   1        full   10G    40GBASE-SR4                    
Et50/1     ANET201-GW WAN connected    routed   full   10G    100GBASE-CR4                   
Et50/2     ANET202-GW WAN connected    routed   full   10G    100GBASE-CR4                   
Et50/3     Cisco45-GW WAN connected    routed   full   10G    100GBASE-CR4                   
Et50/4     Cisco46-GW WAN connected    routed   full   10G    100GBASE-CR4                   
Et51/1                    notconnect   1        full   100G   Not Present                    
Et52/1                    notconnect   1        full   100G   Not Present                    
Et53/1                    disabled     1        full   100G   Not Present                    
Et54/1                    disabled     1        full   100G   Not Present                    
Ma1                       connected    routed   a-full a-1G   10/100/1000                    
Po100                     notconnect   trunk    full   unconf N/A                            
Po200                     connected    trunk    full   20G    N/A                            
Po300                     notconnect   trunk    full   unconf N/A                            
Po301                     notconnect   trunk    full   unconf N/A                            
Po302                     notconnect   1        full   unconf N/A                            

```

## show lldp neighbors

```text
Last table change time   : 0:06:13 ago
Number of table inserts  : 40
Number of table deletes  : 25
Number of table drops    : 0
Number of table age-outs : 0

Port            Neighbor Device ID              Neighbor Port ID        TTL
------------ ------------------------------- -------------------------- ---
Et3             PE13-T3-203.ns.eantc.de         Ethernet5               120
Et13            Cisco_45_N9K-C93240YC-FX2       Ethernet1/5             120
Et14            Cisco_46_N9K-C93240YC-FX2       Ethernet1/5             120
Et15            Cisco_40_N9K-C93180YC-FX3       Ethernet1/5             120
Et16            Cisco_42_N9K-C93400LD-H1        Ethernet1/5             120
Et17            Cisco_44_N3K-C36180YC-R         Ethernet1/5             120
Et21            185b.0089.c3cc                  1610899587              121
Et26            h3c_22_S6850-56HF               Twenty-FiveGigE1/0/3    121
Et48            SPINE1-J-200.ns.eantc.de        Ethernet48              120
Et49/2          juniper-314-ACX7509             et-2/0/4                120
Et50/1          PE11-JP-201.ns.eantc.de         Ethernet10              120
Et50/2          PE12-JP-202.ns.eantc.de         Ethernet10              120
Et50/3          Cisco_45_N9K-C93240YC-FX2       Ethernet1/34            120
Et50/4          Cisco_46_N9K-C93240YC-FX2       Ethernet1/34            120
Ma1             extreme-x460-1                  24                      120

```

