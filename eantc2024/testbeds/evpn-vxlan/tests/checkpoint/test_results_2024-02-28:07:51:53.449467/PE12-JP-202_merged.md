# Test results for PE12-JP-202

## show version

```text
Arista DCS-7280SR3K-48YC8-F
Hardware version: 11.02
Serial number: JPE21115970
Hardware MAC address: 2cdd.e90b.25b7
System MAC address: 2cdd.e90b.25b7

Software image version: 4.32.0F-35483270.hudsonrel (engineering build)
Architecture: x86_64
Internal build version: 4.32.0F-35483270.hudsonrel
Internal build ID: bc4c8e97-b142-4c39-a634-2b265e10ac86
Image format version: 3.0
Image optimization: Default

Uptime: 1 day, 19 hours and 28 minutes
Total memory: 65734516 kB
Free memory: 61828380 kB

```

## show interfaces status

```text
Port       Name           Status       Vlan     Duplex Speed  Type         Flags Encapsulation
Et1        A-Spine-200    notconnect   routed   full   10G    10GBASE-SRL                    
Et2                       notconnect   1        full   10G    Not Present                    
Et3                       notconnect   1        full   10G    Not Present                    
Et4                       notconnect   1        full   10G    Not Present                    
Et5        A-Harn-205     errdisabled  in Po100 full   10G    10GBASE-SRL                    
Et6                       notconnect   1        full   25G    Not Present                    
Et7                       notconnect   1        full   10G    Not Present                    
Et8                       notconnect   1        full   10G    Not Present                    
Et9                       notconnect   1        full   10G    Not Present                    
Et10       SPINE_REMOTE   notconnect   routed   full   10G    25GBASE-CR                     
Et11                      notconnect   1        full   25G    Not Present                    
Et12                      notconnect   1        full   25G    Not Present                    
Et13                      notconnect   1        full   25G    Not Present                    
Et14                      notconnect   1        full   25G    Not Present                    
Et15                      notconnect   1        full   25G    Not Present                    
Et16                      notconnect   1        full   25G    Not Present                    
Et17                      notconnect   1        full   25G    Not Present                    
Et18                      notconnect   1        full   25G    Not Present                    
Et19                      notconnect   1        full   25G    Not Present                    
Et20                      notconnect   1        full   25G    Not Present                    
Et21                      notconnect   1        full   25G    Not Present                    
Et22                      notconnect   1        full   25G    Not Present                    
Et23                      notconnect   1        full   25G    Not Present                    
Et24                      notconnect   1        full   25G    Not Present                    
Et25                      notconnect   1        full   25G    Not Present                    
Et26                      notconnect   1        full   25G    Not Present                    
Et27                      notconnect   1        full   25G    Not Present                    
Et28                      notconnect   1        full   25G    Not Present                    
Et29                      notconnect   1        full   25G    Not Present                    
Et30                      notconnect   1        full   25G    Not Present                    
Et31                      notconnect   1        full   25G    Not Present                    
Et32                      notconnect   1        full   25G    Not Present                    
Et33                      notconnect   1        full   25G    Not Present                    
Et34                      notconnect   1        full   25G    Not Present                    
Et35                      notconnect   1        full   25G    Not Present                    
Et36                      notconnect   1        full   25G    Not Present                    
Et37                      notconnect   1        full   25G    Not Present                    
Et38                      notconnect   1        full   25G    Not Present                    
Et39                      notconnect   1        full   25G    Not Present                    
Et40                      notconnect   1        full   25G    Not Present                    
Et41                      notconnect   1        full   25G    Not Present                    
Et42                      notconnect   1        full   25G    Not Present                    
Et43                      notconnect   1        full   25G    Not Present                    
Et44                      notconnect   1        full   25G    Not Present                    
Et45                      notconnect   1        full   25G    Not Present                    
Et46                      notconnect   1        full   25G    Not Present                    
Et47                      notconnect   1        full   25G    Not Present                    
Et48       Cisco-40-Spine connected    routed   full   10G    10GBASE-AR                     
Et49/1     Nokia-PEG      connected    routed   full   10G    40GBASE-SR4                    
Et49/2                    disabled     1        full   10G    40GBASE-SR4                    
Et49/3                    notconnect   1        full   10G    40GBASE-SR4                    
Et49/4                    notconnect   1        full   10G    40GBASE-SR4                    
Et50/1                    notconnect   1        full   100G   Not Present                    
Et51/1                    notconnect   1        full   100G   Not Present                    
Et52/1                    notconnect   1        full   100G   Not Present                    
Et53/1                    notconnect   1        full   100G   Not Present                    
Et54/1                    notconnect   1        full   40G    Not Present                    
Et55/1                    notconnect   1        full   100G   Not Present                    
Et56/1                    notconnect   1        full   100G   Not Present                    
Ma1                       connected    routed   a-full a-1G   10/100/1000                    
Po100                     disabled     trunk    full   unconf N/A                            

```

## show lldp neighbors

```text
Last table change time   : 14:29:21 ago
Number of table inserts  : 11
Number of table deletes  : 9
Number of table drops    : 0
Number of table age-outs : 0

Port          Neighbor Device ID              Neighbor Port ID    TTL
---------- ------------------------------- ---------------------- ---
Et48          Cisco_40_N9K-C93180YC-FX3       Ethernet1/26        120
Ma1           extreme-x460-1                  29                  120

```

