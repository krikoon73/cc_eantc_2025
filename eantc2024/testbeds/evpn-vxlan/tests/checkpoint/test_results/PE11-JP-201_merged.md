# Test results for PE11-JP-201

## show version

```text
Arista DCS-7280SR2A-48YC6-F
Hardware version: 20.04
Serial number: SSJ17095073
Hardware MAC address: 2899.3a8f.8f6f
System MAC address: 2899.3a8f.8f6f

Software image version: 4.32.0F-35483270.hudsonrel (engineering build)
Architecture: x86_64
Internal build version: 4.32.0F-35483270.hudsonrel
Internal build ID: bc4c8e97-b142-4c39-a634-2b265e10ac86
Image format version: 3.0
Image optimization: Sand-4GB

Uptime: 3 hours and 53 minutes
Total memory: 8051592 kB
Free memory: 5134748 kB

```

## show interfaces status

```text
Port       Name        Status       Vlan     Duplex Speed  Type         Flags Encapsulation
Et1        A-Spine-200 connected    routed   full   10G    10GBASE-SRL                    
Et2                    notconnect   1        full   10G    Not Present                    
Et3                    notconnect   1        full   10G    Not Present                    
Et4                    notconnect   1        full   10G    Not Present                    
Et5        A-Harn-205  disabled     in Po100 full   10G    10GBASE-SRL                    
Et6                    notconnect   1        full   10G    Not Present                    
Et7                    notconnect   1        full   10G    Not Present                    
Et8                    notconnect   1        full   10G    Not Present                    
Et9                    notconnect   1        full   10G    Not Present                    
Et10                   notconnect   routed   full   10G    Not Present                    
Et11                   notconnect   1        full   10G    Not Present                    
Et12                   notconnect   1        full   10G    Not Present                    
Et13                   notconnect   1        full   10G    Not Present                    
Et14                   notconnect   1        full   10G    Not Present                    
Et15                   notconnect   1        full   10G    Not Present                    
Et16                   notconnect   1        full   10G    Not Present                    
Et17                   notconnect   1        full   10G    Not Present                    
Et18                   notconnect   1        full   10G    Not Present                    
Et19                   notconnect   1        full   10G    Not Present                    
Et20                   notconnect   1        full   10G    Not Present                    
Et21                   notconnect   1        full   10G    Not Present                    
Et22                   notconnect   1        full   10G    Not Present                    
Et23                   notconnect   1        full   10G    Not Present                    
Et24                   notconnect   1        full   10G    Not Present                    
Et25                   notconnect   1        full   10G    Not Present                    
Et26                   notconnect   1        full   10G    Not Present                    
Et27                   notconnect   1        full   10G    Not Present                    
Et28                   notconnect   1        full   10G    Not Present                    
Et29                   notconnect   1        full   10G    Not Present                    
Et30                   notconnect   1        full   10G    Not Present                    
Et31                   notconnect   1        full   10G    Not Present                    
Et32                   notconnect   1        full   10G    Not Present                    
Et33                   notconnect   1        full   10G    Not Present                    
Et34                   notconnect   1        full   10G    Not Present                    
Et35                   notconnect   1        full   10G    Not Present                    
Et36                   notconnect   1        full   10G    Not Present                    
Et37                   notconnect   1        full   10G    Not Present                    
Et38                   notconnect   1        full   10G    Not Present                    
Et39                   notconnect   1        full   10G    Not Present                    
Et40                   notconnect   1        full   10G    Not Present                    
Et41                   notconnect   1        full   10G    Not Present                    
Et42                   notconnect   1        full   10G    Not Present                    
Et43                   notconnect   1        full   10G    Not Present                    
Et44                   notconnect   1        full   10G    Not Present                    
Et45                   notconnect   1        full   10G    Not Present                    
Et46                   notconnect   1        full   10G    Not Present                    
Et47                   connected    1        full   10G    10GBASE-SRL                    
Et48                   notconnect   1        full   10G    10GBASE-SRL                    
Et49/1                 notconnect   1        full   100G   Not Present                    
Et50/1                 notconnect   1        full   100G   Not Present                    
Et51/1                 notconnect   1        full   100G   Not Present                    
Et52/1                 notconnect   1        full   100G   Not Present                    
Et53/1                 notconnect   1        full   100G   Not Present                    
Et54/1                 notconnect   1        full   100G   Not Present                    
Ma1                    connected    routed   a-full a-1G   10/100/1000                    
Po100                  notconnect   trunk    full   unconf N/A                            

```

## show lldp neighbors

```text
Last table change time   : 0:46:47 ago
Number of table inserts  : 5
Number of table deletes  : 2
Number of table drops    : 0
Number of table age-outs : 0

Port          Neighbor Device ID             Neighbor Port ID    TTL
---------- ------------------------------ ---------------------- ---
Et1           Spine2-J-180.ns.eantc.de       Ethernet1           120
Et47          PE22-J2-182.ns.eantc.de        Ethernet47          120
Ma1           extreme-x460-1                 25                  120

```

