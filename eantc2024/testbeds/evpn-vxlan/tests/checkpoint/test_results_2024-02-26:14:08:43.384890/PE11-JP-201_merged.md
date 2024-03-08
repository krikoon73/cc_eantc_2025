# Test results for PE11-JP-201

## show version

```text
Arista DCS-7280SR3K-48YC8-F
Hardware version: 11.02
Serial number: JPE21116007
Hardware MAC address: 2cdd.e90b.2283
System MAC address: 2cdd.e90b.2283

Software image version: 4.32.0F-35483270.hudsonrel (engineering build)
Architecture: x86_64
Internal build version: 4.32.0F-35483270.hudsonrel
Internal build ID: bc4c8e97-b142-4c39-a634-2b265e10ac86
Image format version: 3.0
Image optimization: Default

Uptime: 2 hours and 41 minutes
Total memory: 65734516 kB
Free memory: 61826860 kB

```

## show interfaces status

```text
Port       Name        Status       Vlan     Duplex Speed  Type         Flags Encapsulation
Et1        A-Spine-200 connected    routed   full   10G    10GBASE-SRL                    
Et2                    notconnect   1        full   10G    Not Present                    
Et3                    notconnect   1        full   10G    Not Present                    
Et4                    notconnect   1        full   10G    Not Present                    
Et5        A-Harn-205  disabled     in Po100 full   10G    10GBASE-SRL                    
Et6                    notconnect   1        full   25G    Not Present                    
Et7                    notconnect   1        full   25G    Not Present                    
Et8                    notconnect   1        full   25G    Not Present                    
Et9                    notconnect   1        full   25G    Not Present                    
Et10                   connected    routed   full   10G    25GBASE-CR                     
Et11                   notconnect   1        full   25G    Not Present                    
Et12                   notconnect   1        full   25G    Not Present                    
Et13                   notconnect   1        full   25G    Not Present                    
Et14                   notconnect   1        full   25G    Not Present                    
Et15                   notconnect   1        full   25G    Not Present                    
Et16                   notconnect   1        full   25G    Not Present                    
Et17                   notconnect   1        full   25G    Not Present                    
Et18                   notconnect   1        full   25G    Not Present                    
Et19                   notconnect   1        full   25G    Not Present                    
Et20                   notconnect   1        full   25G    Not Present                    
Et21                   notconnect   1        full   25G    Not Present                    
Et22                   notconnect   1        full   25G    Not Present                    
Et23                   notconnect   1        full   25G    Not Present                    
Et24                   notconnect   1        full   25G    Not Present                    
Et25                   notconnect   1        full   25G    Not Present                    
Et26                   notconnect   1        full   25G    Not Present                    
Et27                   notconnect   1        full   25G    Not Present                    
Et28                   notconnect   1        full   25G    Not Present                    
Et29                   notconnect   1        full   25G    Not Present                    
Et30                   notconnect   1        full   25G    Not Present                    
Et31                   notconnect   1        full   25G    Not Present                    
Et32                   notconnect   1        full   25G    Not Present                    
Et33                   notconnect   1        full   25G    Not Present                    
Et34                   notconnect   1        full   25G    Not Present                    
Et35                   notconnect   1        full   25G    Not Present                    
Et36                   notconnect   1        full   25G    Not Present                    
Et37                   notconnect   1        full   25G    Not Present                    
Et38                   notconnect   1        full   25G    Not Present                    
Et39                   notconnect   1        full   25G    Not Present                    
Et40                   notconnect   1        full   25G    Not Present                    
Et41                   notconnect   1        full   25G    Not Present                    
Et42                   notconnect   1        full   25G    Not Present                    
Et43                   notconnect   1        full   25G    Not Present                    
Et44                   notconnect   1        full   25G    Not Present                    
Et45                   notconnect   1        full   25G    Not Present                    
Et46                   notconnect   1        full   25G    Not Present                    
Et47                   notconnect   1        full   25G    Not Present                    
Et48                   notconnect   1        full   25G    Not Present                    
Et49/1                 notconnect   1        full   100G   Not Present                    
Et50/1                 notconnect   1        full   100G   Not Present                    
Et51/1                 notconnect   1        full   100G   Not Present                    
Et52/1                 notconnect   1        full   100G   Not Present                    
Et53/1                 notconnect   1        full   100G   Not Present                    
Et54/1                 notconnect   1        full   100G   Not Present                    
Et55/1                 notconnect   1        full   100G   Not Present                    
Et56/1                 notconnect   1        full   100G   Not Present                    
Ma1                    connected    routed   a-full a-1G   10/100/1000                    
Po100                  notconnect   trunk    full   unconf N/A                            

```

## show lldp neighbors

```text
Last table change time   : 0:09:38 ago
Number of table inserts  : 4
Number of table deletes  : 1
Number of table drops    : 0
Number of table age-outs : 0

Port          Neighbor Device ID               Neighbor Port ID    TTL
---------- -------------------------------- ---------------------- ---
Et1           SPINE1-J-200.ns.eantc.de         Ethernet1           120
Et10          Harness1-J-205.ns.eantc.de       Ethernet50/1        120
Ma1           extreme-x460-1                   28                  120

```

