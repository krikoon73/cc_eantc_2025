# Test results for Harness3-J-175

## show version

```text
Arista DCS-7280SR-48C6-F
Hardware version: 11.03
Serial number: SSJ16420844
Hardware MAC address: 2899.3abe.9402
System MAC address: 2899.3abe.9402

Software image version: 4.31.2F
Architecture: i686
Internal build version: 4.31.2F-35442146.4312F
Internal build ID: 635a071a-386e-447f-942c-bcc34d9ffd3c
Image format version: 3.0
Image optimization: Sand-4GB

Uptime: 1 day, 17 hours and 6 minutes
Total memory: 8051592 kB
Free memory: 5952064 kB

```

## show interfaces status

```text
Port       Name           Status       Vlan     Duplex Speed  Type         Flags Encapsulation
Et1        Arista_171     connected    171      full   10G    10GBASE-SRL                    
Et2        ARISTA_172     connected    172      full   10G    10GBASE-SRL                    
Et3                       connected    1        full   10G    10GBASE-SRL                    
Et4                       disabled     1        full   10G    10GBASE-SRL                    
Et5                       notconnect   1        full   10G    Not Present                    
Et6                       notconnect   1        full   10G    Not Present                    
Et7                       notconnect   1        full   10G    Not Present                    
Et8                       notconnect   1        full   10G    Not Present                    
Et9                       notconnect   1        full   10G    Not Present                    
Et10                      notconnect   1        full   10G    Not Present                    
Et11                      notconnect   1        full   10G    Not Present                    
Et12                      notconnect   1        full   10G    Not Present                    
Et13                      notconnect   1        full   10G    Not Present                    
Et14                      notconnect   1        full   10G    Not Present                    
Et15                      notconnect   1        full   10G    Not Present                    
Et16                      notconnect   1        full   10G    Not Present                    
Et17                      notconnect   1        full   10G    Not Present                    
Et18                      notconnect   1        full   10G    Not Present                    
Et19                      notconnect   1        full   10G    Not Present                    
Et20                      notconnect   1        full   10G    Not Present                    
Et21       Ciena_5        connected    in Po21  full   10G    10GBASE-SRL                    
Et22                      notconnect   1        full   10G    Not Present                    
Et23       Ixia_111       connected    trunk    full   10G    10GBASE-LR                     
Et24                      notconnect   1        full   10G    Not Present                    
Et25       Juniper_379    connected    379      full   10G    10GBASE-LR                     
Et26       Ericson_47     connected    47       full   10G    10GBASE-LR                     
Et27                      notconnect   1        full   10G    Not Present                    
Et28                      notconnect   1        full   10G    Not Present                    
Et29                      notconnect   1        full   10G    Not Present                    
Et30                      notconnect   1        full   10G    Not Present                    
Et31       Juniper_333    connected    333      full   10G    10GBASE-LR                     
Et32                      notconnect   1        full   10G    Not Present                    
Et33                      notconnect   1        full   10G    Not Present                    
Et34                      notconnect   1        full   10G    Not Present                    
Et35                      notconnect   1        full   10G    Not Present                    
Et36                      notconnect   1        full   10G    Not Present                    
Et37                      notconnect   1        full   10G    Not Present                    
Et38                      notconnect   1        full   10G    Not Present                    
Et39                      notconnect   1        full   10G    Not Present                    
Et40       Juniper_server connected    83       full   10G    10GBASE-SRL                    
Et40.1                    notconnect   inactive full   10G    subinterface                   
Et41       Ribbon         connected    32       full   10G    10GBASE-SRL                    
Et42                      notconnect   1        full   10G    Not Present                    
Et43       Cisco_343      connected    343      full   10G    10GBASE-SRL                    
Et44       Nokia_57       connected    57       full   10G    10GBASE-SRL                    
Et45       SPINE_SNIFFER  connected    1        full   10G    10GBASE-SRL                    
Et46       H3C_19         connected    19       full   10G    10GBASE-SRL                    
Et47                      notconnect   1        full   10G    Not Present                    
Et48       Huawei_254     connected    254      full   10G    10GBASE-SRL                    
Et49/1     Cisco_355      connected    355      full   100G   100GBASE-SR4                   
Et50/1                    notconnect   1        full   100G   Not Present                    
Et51/1                    notconnect   1        full   100G   Not Present                    
Et52/1                    notconnect   1        full   100G   Not Present                    
Et53/1                    notconnect   1        full   100G   Not Present                    
Et54/1     H3C_24         connected    24       full   100G   100GBASE-SR4                   
Ma1                       connected    routed   a-full a-1G   10/100/1000                    
Po21                      connected    5        full   10G    N/A                            

```

## show lldp neighbors

```text
Last table change time   : 3:52:11 ago
Number of table inserts  : 34
Number of table deletes  : 19
Number of table drops    : 0
Number of table age-outs : 2

Port          Neighbor Device ID                Neighbor Port ID            TTL
----------- --------------------------------- ----------------------------- ---
Et1           PE31-J2-171.ns.eantc.de           Ethernet5                   120
Et2           PE32-J2-172.ns.eantc.de           Ethernet5                   120
Et3           PE41-J2-161.ns.eantc.de           Ethernet5                   120
Et21          CIEN-5169-5                       3                           120
Et25          juniper_379_MX304                 605                         120
Et31          JNPR-333-PTX10002-36QDD           625                         120
Et40          juniper_303_mx204                 563                         120
Et43          h43-9901                          TenGigE0/0/0/12             120
Et44          NOKIA-SR2-57                      1610899587                  121
Et45          h49-N540-24Q8L2DD                 TenGigE0/0/0/22             120
Et46          h3c_19_CR16010E-F                 Ten-GigabitEthernet2/1/4    121
Et48          huawei_254_NetEngine_8000_F8      GigabitEthernet6/0/9        120
Et49/1        h55-8201-24H8FH                   HundredGigE0/0/0/4          120
Et54/1        h3c_24_S12500R-48C6D              HundredGigE1/0/1            121
Ma1           extreme-x460-1                    40                          120

```

