# Test results for PE31-J2-171

## show version

```text
Arista DCS-7280SR3K-48YC8-F
Hardware version: 11.02
Serial number: JPE21241259
Hardware MAC address: 2cdd.e996.1ab3
System MAC address: 2cdd.e996.1ab3

Software image version: 4.31.2F-35649835.comcasteftfeb24 (engineering build)
Architecture: x86_64
Internal build version: 4.31.2F-35649835.comcasteftfeb24
Internal build ID: 99d2ae30-8d92-4936-8f11-3c8d90acdcf0
Image format version: 3.0
Image optimization: Default

Uptime: 1 day, 15 hours and 15 minutes
Total memory: 65734516 kB
Free memory: 61601744 kB

```

## show interfaces status

```text
Port       Name             Status       Vlan     Duplex Speed  Type                Flags Encapsulation
Et1        Arista_Spine_170 notconnect   routed   full   10G    10GBASE-SRL                           
Et2                         notconnect   1        full   25G    Not Present                           
Et3                         notconnect   routed   full   25G    Not Present                           
Et4                         notconnect   routed   full   25G    Not Present                           
Et5                         connected    routed   full   10G    10GBASE-SRL                           
Et5.1                       connected    routed   full   10G    dot1q-encapsulation       1           
Et5.128                     connected    routed   full   10G    dot1q-encapsulation       128         
Et5.129                     connected    routed   full   10G    dot1q-encapsulation       129         
Et5.130                     connected    routed   full   10G    dot1q-encapsulation       130         
Et5.131                     connected    routed   full   10G    dot1q-encapsulation       131         
Et6                         notconnect   1        full   25G    Not Present                           
Et7        Ribbon           notconnect   routed   full   10G    10GBASE-SRL                           
Et8                         notconnect   1        full   25G    Not Present                           
Et9        HUwaii_254       disabled     routed   full   10G    10GBASE-SRL                           
Et10                        notconnect   1        full   25G    Not Present                           
Et11                        notconnect   1        full   25G    Not Present                           
Et12                        notconnect   1        full   25G    Not Present                           
Et13                        notconnect   1        full   25G    Not Present                           
Et14                        notconnect   1        full   25G    Not Present                           
Et15                        notconnect   1        full   25G    Not Present                           
Et16                        notconnect   1        full   25G    Not Present                           
Et17                        notconnect   1        full   25G    Not Present                           
Et18                        notconnect   1        full   25G    Not Present                           
Et19                        notconnect   1        full   25G    Not Present                           
Et20                        notconnect   1        full   25G    Not Present                           
Et21                        notconnect   1        full   25G    Not Present                           
Et22                        notconnect   1        full   25G    Not Present                           
Et23                        notconnect   1        full   25G    Not Present                           
Et24       Cisco_Spine_349  disabled     routed   full   10G    10GBASE-SRL                           
Et25       Juniper_TWAMP    disabled     routed   full   10G    10GBASE-LR                            
Et26                        notconnect   1        full   25G    Not Present                           
Et27                        notconnect   1        full   25G    Not Present                           
Et28                        notconnect   1        full   25G    Not Present                           
Et29                        notconnect   1        full   25G    Not Present                           
Et30                        notconnect   1        full   25G    Not Present                           
Et31                        notconnect   1        full   25G    Not Present                           
Et32                        notconnect   1        full   25G    Not Present                           
Et33                        notconnect   1        full   25G    Not Present                           
Et34                        notconnect   1        full   25G    Not Present                           
Et35                        notconnect   1        full   25G    Not Present                           
Et36                        notconnect   1        full   25G    Not Present                           
Et37                        notconnect   1        full   25G    Not Present                           
Et38                        notconnect   1        full   25G    Not Present                           
Et39                        notconnect   1        full   25G    Not Present                           
Et40                        notconnect   1        full   25G    Not Present                           
Et41                        notconnect   1        full   25G    Not Present                           
Et42                        notconnect   1        full   25G    Not Present                           
Et43                        notconnect   1        full   25G    Not Present                           
Et44                        notconnect   1        full   25G    Not Present                           
Et45                        notconnect   1        full   25G    Not Present                           
Et46                        disabled     routed   full   10G    10GBASE-SRL                           
Et47                        notconnect   routed   full   10G    10GBASE-SRL                           
Et48                        connected    routed   full   10G    10GBASE-SRL                           
Et49/1     Nokia_57         connected    routed   full   10G    40GBASE-SR4                           
Et49/2                      notconnect   1        full   10G    40GBASE-SR4                           
Et49/3                      notconnect   1        full   10G    40GBASE-SR4                           
Et49/4                      notconnect   1        full   10G    40GBASE-SR4                           
Et50/1                      notconnect   1        full   100G   Not Present                           
Et51/1                      notconnect   1        full   100G   Not Present                           
Et52/1                      notconnect   1        full   100G   Not Present                           
Et53/1                      notconnect   1        full   100G   Not Present                           
Et54/1                      notconnect   1        full   100G   Not Present                           
Et55/1                      notconnect   1        full   100G   Not Present                           
Et56/1                      notconnect   1        full   100G   Not Present                           
Ma1                         connected    routed   a-full a-1G   10/100/1000                           

```

## show lldp neighbors

```text
Last table change time   : 15:59:35 ago
Number of table inserts  : 13
Number of table deletes  : 9
Number of table drops    : 0
Number of table age-outs : 0

Port            Neighbor Device ID               Neighbor Port ID    TTL
------------ -------------------------------- ---------------------- ---
Et5             Harness3-J-175.ns.eantc.de       Ethernet1           120
Et48            PE32-J2-172.ns.eantc.de          Ethernet48          120
Et49/1          NOKIA-SR2-57                     1610899526          121
Ma1             extreme-x460-1                   34                  120

```

