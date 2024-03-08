# Test results for PE32-J2-172

## show version

```text
Arista DCS-7280SR3-48YC8-F
Hardware version: 12.01
Serial number: JPE21210788
Hardware MAC address: 2cdd.e996.3abb
System MAC address: 2cdd.e996.3abb

Software image version: 4.31.2F
Architecture: i686
Internal build version: 4.31.2F-35442146.4312F
Internal build ID: 635a071a-386e-447f-942c-bcc34d9ffd3c
Image format version: 3.0
Image optimization: Default

Uptime: 16 hours and 55 minutes
Total memory: 8099732 kB
Free memory: 5552204 kB

```

## show interfaces status

```text
Port       Name        Status       Vlan     Duplex Speed  Type                Flags Encapsulation
Et1                    notconnect   1        full   10G    10GBASE-SRL                           
Et2                    notconnect   1        full   25G    Not Present                           
Et3                    notconnect   1        full   25G    Not Present                           
Et4                    notconnect   1        full   25G    Not Present                           
Et5                    connected    routed   full   10G    10GBASE-SRL                           
Et5.2                  connected    routed   full   10G    dot1q-encapsulation       2           
Et5.3                  notconnect   routed   full   10G    Unknown                               
Et5.171                connected    routed   full   10G    dot1q-encapsulation       172         
Et5.172                notconnect   routed   full   10G    Unknown                               
Et6                    notconnect   1        full   25G    Not Present                           
Et7                    notconnect   1        full   25G    Not Present                           
Et8                    notconnect   1        full   25G    Not Present                           
Et9                    notconnect   1        full   25G    Not Present                           
Et10                   notconnect   1        full   25G    Not Present                           
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
Et45       Juniper_311 notconnect   routed   full   25G    Not Present                           
Et46                   notconnect   1        full   25G    Not Present                           
Et47       Arista_171  disabled     routed   full   10G    10GBASE-SRL                           
Et48                   connected    1        full   10G    10GBASE-SRL                           
Et49/1     Nokia_57    disabled     routed   full   10G    40GBASE-SR4                           
Et49/2                 notconnect   1        full   10G    40GBASE-SR4                           
Et49/3                 notconnect   1        full   10G    40GBASE-SR4                           
Et49/4                 notconnect   1        full   10G    40GBASE-SR4                           
Et50/1     Ribbon_32   disabled     routed   full   10G    40GBASE-SR4                           
Et50/2                 notconnect   1        full   10G    40GBASE-SR4                           
Et50/3                 notconnect   1        full   10G    40GBASE-SR4                           
Et50/4                 notconnect   1        full   10G    40GBASE-SR4                           
Et51/1     ERIKSON_47  connected    routed   full   100G   100GBASE-SR4                          
Et52/1                 notconnect   1        full   10G    Not Present                           
Et52/2                 notconnect   1        full   25G    Not Present                           
Et52/3                 notconnect   1        full   25G    Not Present                           
Et52/4                 notconnect   1        full   25G    Not Present                           
Et53/1                 notconnect   1        full   10G    Not Present                           
Et53/2                 notconnect   1        full   25G    Not Present                           
Et53/3                 notconnect   1        full   25G    Not Present                           
Et53/4                 notconnect   1        full   25G    Not Present                           
Et54/1                 notconnect   1        full   10G    Not Present                           
Et54/2                 notconnect   1        full   25G    Not Present                           
Et54/3                 notconnect   1        full   25G    Not Present                           
Et54/4                 notconnect   1        full   25G    Not Present                           
Et55/1     H3C_19      connected    routed   full   100G   100GBASE-SR4                          
Et56/1                 notconnect   1        full   10G    Not Present                           
Et56/2                 notconnect   1        full   25G    Not Present                           
Et56/3                 notconnect   1        full   25G    Not Present                           
Et56/4                 notconnect   1        full   25G    Not Present                           
Ma1                    connected    routed   a-full a-1G   10/100/1000                           

```

## show lldp neighbors

```text
Last table change time   : 0:49:00 ago
Number of table inserts  : 5
Number of table deletes  : 1
Number of table drops    : 0
Number of table age-outs : 0

Port            Neighbor Device ID               Neighbor Port ID    TTL
------------ -------------------------------- ---------------------- ---
Et5             Harness3-J-175.ns.eantc.de       Ethernet2           120
Et48            PE31-J2-171.ns.eantc.de          Ethernet48          120
Et55/1          h3c_19_CR16010E-F                HundredGigE2/2/1    121
Ma1             extreme-x460-1                   39                  120

```

