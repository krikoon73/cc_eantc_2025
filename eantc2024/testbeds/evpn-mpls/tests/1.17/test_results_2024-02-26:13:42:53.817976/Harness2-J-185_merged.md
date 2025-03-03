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
   4    0013.0100.0001    DYNAMIC     Et47       1       4:51:28 ago
   4    0013.0100.0002    DYNAMIC     Et47       1       4:51:28 ago
   4    0013.0100.0003    DYNAMIC     Et47       1       4:51:28 ago
   4    0013.0100.0004    DYNAMIC     Et47       1       4:51:28 ago
   4    0013.0100.0005    DYNAMIC     Et47       1       4:51:28 ago
   4    0056.5656.5656    DYNAMIC     Et11       1       4:00:46 ago
   4    00aa.aaaa.aaaa    DYNAMIC     Et11       1       4:51:28 ago
   4    30c5.071f.43ef    DYNAMIC     Et11       1       4:00:46 ago
   4    e4f2.7cef.a505    DYNAMIC     Et11       1       4:00:46 ago
  21    001a.0100.0004    DYNAMIC     Et47       1       2:30:03 ago
  21    001a.0100.0005    DYNAMIC     Et47       1       2:28:16 ago
  21    0056.5656.5656    DYNAMIC     Po21       1       0:13:38 ago
  21    00aa.aaaa.aaaa    DYNAMIC     Po21       1       2:43:31 ago
  21    30c5.071f.43ef    DYNAMIC     Po21       1       0:12:02 ago
  21    e4f2.7cef.a505    DYNAMIC     Po21       1       2:28:14 ago
  26    0000.3f3d.4889    DYNAMIC     Po26       1       0:13:28 ago
  26    0019.0100.0004    DYNAMIC     Et47       1       4:02:06 ago
  26    0019.0100.0005    DYNAMIC     Et47       1       4:00:46 ago
  26    0056.5656.5656    DYNAMIC     Po26       1       4:00:46 ago
  26    00aa.aaaa.aaaa    DYNAMIC     Po26       1       4:18:42 ago
  26    e4f2.7cef.a505    DYNAMIC     Po26       1       4:00:46 ago
  31    0014.0100.0001    DYNAMIC     Et47       1       4:51:28 ago
  31    0014.0100.0002    DYNAMIC     Et47       1       4:51:28 ago
  31    0014.0100.0003    DYNAMIC     Et47       1       4:51:28 ago
  31    0014.0100.0004    DYNAMIC     Et47       1       4:51:28 ago
  31    0014.0100.0005    DYNAMIC     Et47       1       4:51:28 ago
  31    0056.5656.5656    DYNAMIC     Et15       1       4:00:46 ago
  31    00aa.aaaa.aaaa    DYNAMIC     Et15       1       4:51:28 ago
  31    30c5.071f.43ef    DYNAMIC     Et15       1       4:00:46 ago
  31    e4f2.7cef.a505    DYNAMIC     Et15       1       4:00:46 ago
  32    0014.0100.0002    DYNAMIC     Po32       1       4:51:28 ago
  32    0014.0100.0003    DYNAMIC     Po32       1       4:51:28 ago
  32    0014.0100.0004    DYNAMIC     Po32       1       4:51:28 ago
  32    0014.0100.0005    DYNAMIC     Po32       1       4:51:28 ago
  32    0015.0100.0004    DYNAMIC     Et47       1       4:04:50 ago
  32    0015.0100.0005    DYNAMIC     Et47       1       4:00:46 ago
  32    00aa.aaaa.aaaa    DYNAMIC     Po32       1       0:59:37 ago
  32    60c7.8d2d.4416    DYNAMIC     Po32       1       0:40:26 ago
  33    0014.0100.0004    DYNAMIC     Po33       1       4:51:28 ago
  33    0014.0100.0005    DYNAMIC     Po33       1       4:51:28 ago
  33    001b.0100.0004    DYNAMIC     Et47       1       4:02:06 ago
  33    001b.0100.0005    DYNAMIC     Et47       1       4:03:38 ago
  33    00aa.aaaa.aaaa    DYNAMIC     Po33       1       4:18:42 ago
  33    e4f2.7cef.a505    DYNAMIC     Po33       1       0:48:43 ago
  56    0018.0100.0004    DYNAMIC     Et47       1       4:03:42 ago
  56    0018.0100.0005    DYNAMIC     Et47       1       4:02:12 ago
  56    0056.5656.5656    DYNAMIC     Et21       1       4:00:46 ago
  56    00aa.aaaa.aaaa    DYNAMIC     Et21       1       4:18:42 ago
  56    30c5.071f.43ef    DYNAMIC     Et21       1       4:00:46 ago
  68    0012.0100.0001    DYNAMIC     Et47       1       4:51:28 ago
  68    0012.0100.0002    DYNAMIC     Et47       1       4:51:28 ago
  68    0012.0100.0003    DYNAMIC     Et47       1       4:51:28 ago
  68    0012.0100.0004    DYNAMIC     Et47       1       4:51:28 ago
  68    0012.0100.0005    DYNAMIC     Et47       1       4:51:28 ago
  68    0014.0100.0002    DYNAMIC     Po68       1       4:51:28 ago
  68    0014.0100.0003    DYNAMIC     Po68       1       4:51:28 ago
  68    0014.0100.0005    DYNAMIC     Po68       1       4:51:28 ago
  68    00aa.aaaa.aaaa    DYNAMIC     Po68       1       4:51:28 ago
  68    c4ca.2b45.ef6d    DYNAMIC     Po68       1       4:00:46 ago
  68    e4f2.7cef.a505    DYNAMIC     Po68       1       4:00:46 ago
Total Mac Addresses for this criterion: 60

          Multicast Mac Address Table
------------------------------------------------------------------

Vlan    Mac Address       Type        Ports
----    -----------       ----        -----
Total Mac Addresses for this criterion: 0
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

Uptime: 6 hours and 48 minutes
Total memory: 8098968 kB
Free memory: 5607408 kB

```

