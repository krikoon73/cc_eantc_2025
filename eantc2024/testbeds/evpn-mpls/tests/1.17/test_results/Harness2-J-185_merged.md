# Test results for Harness2-J-185

## show bgp evpn

```text
BGP is disabled for VRF default
BGP routing table information for VRF default
Router identifier 0.0.0.0, local AS number 0
Route status codes: s - suppressed, * - valid, > - active, E - ECMP head, e - ECMP
                    S - Stale, c - Contributing to ECMP, b - backup
                    % - Pending BGP convergence
Origin codes: i - IGP, e - EGP, ? - incomplete
AS Path Attributes: Or-ID - Originator ID, C-LST - Cluster List, LL Nexthop - Link Local Nexthop

          Network                Next Hop              Metric  LocPref Weight  Path
```

## show bgp evpn instance

```text
```

## show mac address-table

```text
          Mac Address Table
------------------------------------------------------------------

Vlan    Mac Address       Type        Ports      Moves   Last Move
----    -----------       ----        -----      -----   ---------
   4    0013.0100.0001    DYNAMIC     Et47       1       4:56:28 ago
   4    0013.0100.0002    DYNAMIC     Et47       1       4:56:28 ago
   4    0013.0100.0003    DYNAMIC     Et47       1       4:56:28 ago
   4    0013.0100.0004    DYNAMIC     Et47       1       4:56:28 ago
   4    0013.0100.0005    DYNAMIC     Et47       1       4:56:28 ago
   4    0056.5656.5656    DYNAMIC     Et11       1       4:05:47 ago
   4    00aa.aaaa.aaaa    DYNAMIC     Et11       1       4:56:28 ago
   4    30c5.071f.43ef    DYNAMIC     Et11       1       4:05:47 ago
   4    e4f2.7cef.a505    DYNAMIC     Et11       1       4:05:47 ago
  21    001a.0100.0004    DYNAMIC     Et47       1       2:35:03 ago
  21    001a.0100.0005    DYNAMIC     Et47       1       2:33:17 ago
  21    0056.5656.5656    DYNAMIC     Po21       1       0:18:39 ago
  21    00aa.aaaa.aaaa    DYNAMIC     Po21       1       2:48:31 ago
  21    30c5.071f.43ef    DYNAMIC     Po21       1       0:17:02 ago
  21    e4f2.7cef.a505    DYNAMIC     Po21       1       2:33:15 ago
  26    0000.3f3d.4889    DYNAMIC     Po26       1       0:18:28 ago
  26    0019.0100.0004    DYNAMIC     Et47       1       4:07:07 ago
  26    0019.0100.0005    DYNAMIC     Et47       1       4:05:47 ago
  26    0056.5656.5656    DYNAMIC     Po26       1       4:05:47 ago
  26    00aa.aaaa.aaaa    DYNAMIC     Po26       1       4:23:43 ago
  26    e4f2.7cef.a505    DYNAMIC     Po26       1       4:05:47 ago
  31    0014.0100.0001    DYNAMIC     Et47       1       4:56:28 ago
  31    0014.0100.0002    DYNAMIC     Et47       1       4:56:28 ago
  31    0014.0100.0003    DYNAMIC     Et47       1       4:56:28 ago
  31    0014.0100.0004    DYNAMIC     Et47       1       4:56:28 ago
  31    0014.0100.0005    DYNAMIC     Et47       1       4:56:28 ago
  31    0056.5656.5656    DYNAMIC     Et15       1       4:05:47 ago
  31    00aa.aaaa.aaaa    DYNAMIC     Et15       1       4:56:28 ago
  31    30c5.071f.43ef    DYNAMIC     Et15       1       4:05:47 ago
  31    e4f2.7cef.a505    DYNAMIC     Et15       1       4:05:47 ago
  32    0014.0100.0002    DYNAMIC     Po32       1       4:56:28 ago
  32    0014.0100.0003    DYNAMIC     Po32       1       4:56:28 ago
  32    0014.0100.0004    DYNAMIC     Po32       1       4:56:28 ago
  32    0014.0100.0005    DYNAMIC     Po32       1       4:56:28 ago
  32    0015.0100.0001    DYNAMIC     Et47       1       0:00:28 ago
  32    0015.0100.0002    DYNAMIC     Et47       1       0:02:41 ago
  32    0015.0100.0003    DYNAMIC     Et47       1       0:00:24 ago
  32    0015.0100.0004    DYNAMIC     Et47       1       4:09:50 ago
  32    0015.0100.0005    DYNAMIC     Et47       1       4:05:47 ago
  32    00aa.aaaa.aaaa    DYNAMIC     Po32       1       1:04:38 ago
  32    60c7.8d2d.4416    DYNAMIC     Po32       1       0:45:26 ago
  33    0014.0100.0004    DYNAMIC     Po33       1       4:56:28 ago
  33    0014.0100.0005    DYNAMIC     Po33       1       4:56:28 ago
  33    001b.0100.0004    DYNAMIC     Et47       1       4:07:07 ago
  33    001b.0100.0005    DYNAMIC     Et47       1       4:08:39 ago
  33    00aa.aaaa.aaaa    DYNAMIC     Po33       1       4:23:43 ago
  33    e4f2.7cef.a505    DYNAMIC     Po33       1       0:53:44 ago
  56    0018.0100.0002    DYNAMIC     Et47       1       0:04:07 ago
  56    0018.0100.0003    DYNAMIC     Et47       1       0:04:07 ago
  56    0018.0100.0004    DYNAMIC     Et47       1       4:08:43 ago
  56    0018.0100.0005    DYNAMIC     Et47       1       4:07:13 ago
  56    0056.5656.5656    DYNAMIC     Et21       1       4:05:47 ago
  56    00aa.aaaa.aaaa    DYNAMIC     Et21       1       4:23:43 ago
  56    30c5.071f.43ef    DYNAMIC     Et21       1       4:05:47 ago
  68    0012.0100.0001    DYNAMIC     Et47       1       4:56:28 ago
  68    0012.0100.0002    DYNAMIC     Et47       1       4:56:28 ago
  68    0012.0100.0003    DYNAMIC     Et47       1       4:56:28 ago
  68    0012.0100.0004    DYNAMIC     Et47       1       4:56:28 ago
  68    0012.0100.0005    DYNAMIC     Et47       1       4:56:28 ago
  68    0014.0100.0002    DYNAMIC     Po68       1       4:56:28 ago
  68    0014.0100.0003    DYNAMIC     Po68       1       4:56:28 ago
  68    0014.0100.0005    DYNAMIC     Po68       1       4:56:28 ago
  68    00aa.aaaa.aaaa    DYNAMIC     Po68       1       4:56:28 ago
  68    c4ca.2b45.ef6d    DYNAMIC     Po68       1       4:05:47 ago
  68    e4f2.7cef.a505    DYNAMIC     Po68       1       4:05:47 ago
Total Mac Addresses for this criterion: 65

          Multicast Mac Address Table
------------------------------------------------------------------

Vlan    Mac Address       Type        Ports
----    -----------       ----        -----
Total Mac Addresses for this criterion: 0
```

## show ip route vrf tenant-a

```text

VRF: tenant-a
Codes: C - connected, S - static, K - kernel, 
       O - OSPF, IA - OSPF inter area, E1 - OSPF external type 1,
       E2 - OSPF external type 2, N1 - OSPF NSSA external type 1,
       N2 - OSPF NSSA external type2, B - Other BGP Routes,
       B I - iBGP, B E - eBGP, R - RIP, I L1 - IS-IS level 1,
       I L2 - IS-IS level 2, O3 - OSPFv3, A B - BGP Aggregate,
       A O - OSPF Summary, NG - Nexthop Group Static Route,
       V - VXLAN Control Service, M - Martian,
       DH - DHCP client installed default route,
       DP - Dynamic Policy Route, L - VRF Leaked,
       G  - gRIBI, RC - Route Cache Route

Gateway of last resort is not set


! IP routing not enabled
```

## show ip arp vrf tenant-a

```text
Address         Age (sec)  Hardware Addr   Interface
```

## show mpls label ranges

```text
Start     End       Size      Usage             
------------------------------------------------
0         15        16        reserved          
16        99999     99984     static mpls       
100000    362143    262144    free (dynamic)    
362144    899999    537856    unassigned        
900000    965535    65536     isis-sr           
900000    965535    65536     bgp-sr            
965536    1031071   65536     srlb              
1031072   1032095   1024      l2evpn shared ethernet-segment
1032096   1036287   4192      unassigned        
1036288   1048575   12288     l2evpn            
```

## show version

```text
Arista DCS-7280SR-48C6-F
Hardware version: 10.01
Serial number: JPE17131945
Hardware MAC address: 2899.3a06.b1fd
System MAC address: 2899.3a06.b1fd

Software image version: 4.27.3F
Architecture: x86_64
Internal build version: 4.27.3F-26391011.4273F
Internal build ID: 037a4a3f-ba8d-42a8-8876-433ce8a83555
Image format version: 2.0
Image optimization: DEFAULT

Uptime: 6 hours and 53 minutes
Total memory: 8098968 kB
Free memory: 5596892 kB

```

