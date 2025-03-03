# Test results for PE42-J2-162

## show running-config | no-more

```text
! Command: show running-config
! device: PE42-J2-162 (DCS-7280SR3-40YC6, EOS-4.31.2F)
!
! boot system flash:/EOS-4.31.2F.swi
!
no aaa root
aaa authentication policy local allow-nopassword-remote-login
!
username admin privilege 15 role network-admin nopassword
username eantc privilege 15 role network-admin secret sha512 $6$ZswCmV3GVuWEiesM$ZRvQQUWfypDf9pPCUpT27.0Fi/kf3EGZ9oG5W/ao9.iS/iBtXIrwY4MwabSWuAY6g82op/H91K9bY1wSH17ji.
username magno privilege 15 role network-admin secret sha512 $6$WX8pBInrzoI4ncV1$kFAdCP5wKMB/X5qzP/FeF9zU9f0UkGycuTv2b5j9MHQU/L/Cl.5P3tRq51Q.GH3DqwONRr1/vYxTrZYXiPVdN0
username magno ssh-key ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQDw5erpfpWw/i2M5BW7sB1YHlXQRB/nvZnGcj+L8yhXg0H9mJ86wRf++FWYF2WrdPLGn4aZzBmTl9gifc3+LnYrr1OBK97+EOQbvfg2VO6g0ZcWkTvB0PrLOCEqUTKHg8rwy4hjc3Xq4/pOJeb5w0cJwNW78namqgvvTbf1iPWHMmlzWVuO3Mc9MGFqQdySmG6V3psIgKWeVAZB3f3KznB0LinyQoKHah77xBh8oHtoXDsGxksc538TYJlgw9nnbAxEZ8eOq1vQnnAv7FslzvlHNPRSzoPjr13aN3BPFsYkJ5inmhddvz2Ii66w/UdlyqZvX7hfjZOYWhnmsykdukuD massimo@davideb
!
trace AleL3Agent-primary filename ALE-TRACE.txt
trace Bgp setting BgpParse/*f
trace Bgp filename BGP-DEBUG.txt
!
terminal length 40
terminal width 120
alias ls bash ls -lrt /var/log/agents
alias senz show interface counter error | nz
alias shmc show int | awk '/^[A-Z]/ { intf = $1 } /, address is/ { print intf, $6 }'
alias snz show interface counter | nz
alias spd show port-channel %1 detail all
alias sqnz show interface counter queue | nz
alias srnz show interfaces counters rates | nz
!
load-interval default 5
!
service routing protocols model multi-agent
!
hostname PE42-J2-162
ip name-server vrf mgmt 192.168.100.100
ip name-server vrf mgmt 192.168.160.100
dns domain ns.eantc.de
!
snmp-server community public ro
!
hardware speed-group1 serdes 10g
!
spanning-tree mode mstp
!
service unsupported-transceiver EANTC2024_SRV6 e1ecc879
!
system l1
   unsupported speed action error
   unsupported error-correction action error
!
vlan 20
   name VPNv4-uSID
!
vrf instance EVPN-v6
!
vrf instance EVPNv4-T5-uSID
!
vrf instance IPV6
!
vrf instance VPNv4-uSID
!
vrf instance mgmt
!
management api http-commands
   protocol http
   protocol https ssl profile TLS1.2
   no shutdown
   !
   vrf mgmt
      no shutdown
!
management security
   ssl profile TLS1.2
      tls versions 1.2
      certificate ssl.crt key ssl.key
!
aaa authorization exec default local
aaa authorization commands all default local
!
interface Ethernet1
!
interface Ethernet2
!
interface Ethernet3
!
interface Ethernet4
!
interface Ethernet5
!
interface Ethernet6
!
interface Ethernet7
!
interface Ethernet8
!
interface Ethernet9
!
interface Ethernet10
   shutdown
   mtu 9214
   speed forced 10000full
   no switchport
   ipv6 address 2001:0:162:302::162/64
   isis enable srv6
   isis network point-to-point
!
interface Ethernet11
!
interface Ethernet12
   shutdown
   switchport trunk allowed vlan 20-21
   switchport mode trunk
!
interface Ethernet13
!
interface Ethernet14
!
interface Ethernet15
!
interface Ethernet16
!
interface Ethernet17
!
interface Ethernet18
!
interface Ethernet19
!
interface Ethernet20
   shutdown
   mtu 9214
   no switchport
   ipv6 address 2001:0:162:344::162/64
   isis enable srv6
   isis metric 1000
   isis network point-to-point
!
interface Ethernet21
!
interface Ethernet22
!
interface Ethernet23
!
interface Ethernet24
!
interface Ethernet25
!
interface Ethernet26
!
interface Ethernet27
!
interface Ethernet28
!
interface Ethernet29
!
interface Ethernet30
!
interface Ethernet31
!
interface Ethernet32
!
interface Ethernet33
!
interface Ethernet34
!
interface Ethernet35
!
interface Ethernet36
!
interface Ethernet37
!
interface Ethernet38
!
interface Ethernet39
   shutdown
   speed forced 10000full
!
interface Ethernet40
   shutdown
   speed forced 10000full
!
interface Ethernet41/1
   description Nokia_57
   speed forced 10000full
   no switchport
   ipv6 address 2001:0:57:162::162/64
   isis enable IPV6
   isis metric 10
   isis network point-to-point
!
interface Ethernet41/2
!
interface Ethernet41/3
!
interface Ethernet41/4
!
interface Ethernet43/1
!
interface Ethernet44/1
!
interface Ethernet45/1
!
interface Ethernet46/1
!
interface Loopback0
   description Router-ID
   ip address 100.0.0.162/32
   ipv6 address 2002::162/128
   node-segment ipv4 index 162
   node-segment ipv6 index 1162
   isis instance IPV6
   isis passive
!
interface Loopback100
   vrf IPV6
   ip address 162.162.162.162/32
   ipv6 address 2002:162::162/128
!
interface Loopback101
   vrf EVPN-v6
   ip address 162.162.162.162/32
   ipv6 address 2002:162::162/128
!
interface Management1
   vrf mgmt
   ip address 192.168.20.162/23
!
interface Vlan20
   vrf VPNv4-uSID
   ip address 20.162.225.162/24
   ipv6 address 2001:20:162:225::162/64
!
ip virtual-router mac-address 00:aa:aa:aa:aa:aa
!
ip routing
ip hardware fib hierarchical next-hop max-level 3
ip routing vrf EVPN-v6
ip routing vrf EVPNv4-T5-uSID
ip routing vrf IPV6
ip routing vrf VPNv4-uSID
ip routing vrf mgmt
!
ipv6 unicast-routing
ipv6 unicast-routing vrf EVPN-v6
ipv6 unicast-routing vrf EVPNv4-T5-uSID
ipv6 unicast-routing vrf IPV6
ipv6 unicast-routing vrf VPNv4-uSID
!
monitor session 41-1 source Ethernet41/1
monitor session 41-1 destination Cpu
!
ip route vrf mgmt 0.0.0.0/0 192.168.20.1
!
mpls ip
!
ntp server vrf mgmt 192.168.100.132
!
router bgp 65000
   router-id 100.0.0.162
   no bgp default ipv4-unicast
   bgp default ipv4-unicast transport ipv6
   maximum-paths 4 ecmp 4
   neighbor IBGP-IPV6 peer group
   neighbor IBGP-IPV6 remote-as 65000
   neighbor IBGP-IPV6 next-hop-self
   neighbor IBGP-IPV6 update-source Loopback0
   neighbor IBGP-IPV6 rib-in pre-policy retain all
   neighbor IBGP-IPV6 additional-paths receive
   neighbor IBGP-IPV6 send-community
   neighbor IBGP-IPV6 maximum-routes 0
   neighbor 2002::59 peer group IBGP-IPV6
   neighbor 2002::304 peer group IBGP-IPV6
   !
   address-family evpn
      neighbor default encapsulation mpls next-hop-self source-interface Loopback0
      neighbor IBGP-IPV6 activate
   !
   address-family vpn-ipv4
      next-hop resolution ribs tunnel-rib system-tunnel-rib system-connected
      no neighbor IBGP-IPV6 activate
      neighbor 2002::59 activate
      neighbor default encapsulation mpls next-hop-self source-interface Loopback0
      next-hop resolution ribs vrf-unicast-rib
   !
   address-family vpn-ipv6
      neighbor IBGP-IPV6 activate
      neighbor default encapsulation mpls next-hop-self source-interface Loopback0
   !
   vrf EVPN-v6
      rd 10.0.0.162:162
      route-target import evpn 65000:6001
      route-target import evpn 65000:6002
      route-target export evpn 65000:6001
      route-target export evpn 65000:6002
      redistribute connected
      redistribute static
   !
   vrf IPV6
      rd 10.0.0.162:1
      route-target import vpn-ipv4 65000:6001
      route-target import vpn-ipv6 65000:6001
      route-target export vpn-ipv4 65000:6001
      route-target export vpn-ipv6 65000:6001
      redistribute connected
      redistribute static
!
router traffic-engineering
   segment-routing
      rib system-colored-tunnel-rib
!
router isis IPV6
   hello padding disabled
   net 49.0000.0100.0000.0162.00
   is-hostname anet-PE42-J2-162
   is-type level-2
   timers local-convergence-delay protected-prefixes
   spf-interval 2 10 100
   timers lsp out-delay 2000
   adjacency address-family match disabled
   !
   address-family ipv6 unicast
      fast-reroute ti-lfa mode node-protection
   !
   segment-routing mpls
      router-id 100.0.0.162
      no shutdown
      adjacency-segment allocation all-interfaces
!
end
```

## show version

```text
Arista DCS-7280SR3-40YC6-F
Hardware version: 11.02
Serial number: JPA2339P1QH
Hardware MAC address: 606b.5b2e.f3fd
System MAC address: 606b.5b2e.f3fd

Software image version: 4.31.2F
Architecture: i686
Internal build version: 4.31.2F-35442146.4312F
Internal build ID: 635a071a-386e-447f-942c-bcc34d9ffd3c
Image format version: 3.0
Image optimization: Default

Uptime: 10 hours and 1 minute
Total memory: 8099732 kB
Free memory: 5643820 kB

```

## show lldp neighbors

```text
Last table change time   : 9:34:22 ago
Number of table inserts  : 2
Number of table deletes  : 0
Number of table drops    : 0
Number of table age-outs : 0

Port            Neighbor Device ID       Neighbor Port ID    TTL
------------ ------------------------ ---------------------- ---
Et41/1          NOKIA-SR2-57             1610899526          121
Ma1             extreme-x460-1           22                  120

```

## show bgp summary

```text
BGP summary information for VRF default
Router identifier 100.0.0.162, local AS number 65000
Neighbor           AS Session State AFI/SAFI                AFI/SAFI State   NLRI Rcd   NLRI Acc
--------- ----------- ------------- ----------------------- -------------- ---------- ----------
2002::59        65000 Established   IPv4 Unicast            Advertised              0          0
2002::59        65000 Established   IPv4 MplsVpn            Negotiated             12          5
2002::59        65000 Established   IPv6 MplsVpn            Negotiated              8          8
2002::59        65000 Established   L2VPN EVPN              Negotiated              3          3
2002::304       65000 Established   IPv4 Unicast            Advertised              0          0
2002::304       65000 Established   IPv4 MplsVpn            Received                0          0
2002::304       65000 Established   IPv6 MplsVpn            Negotiated              3          3
2002::304       65000 Established   L2VPN EVPN              Advertised              0          0
```

## show tunnel rib system-tunnel-rib summary

```text
Tunnel RIB: system-tunnel-rib
   Tunnel Type      Tunnel Count
------------------- ------------
   IS-IS SR IPv6               4
                                
   Total tunnels               4

```

## show tunnel rib system-tunnel-rib brief

```text
Tunnel RIB: system-tunnel-rib
Endpoint        Tunnel Type     Index(es)   Tunnel Preference   IGP Preference 
-------------- --------------- ----------- ------------------- ----------------
2002::57/128    IS-IS SR IPv6   2           65                  115            
2002::304/128   IS-IS SR IPv6   4           65                  115            
2002::59/128    IS-IS SR IPv6   1           65                  115            
2002::303/128   IS-IS SR IPv6   3           65                  115            

   IGP Metric    Metric Type
---------------- -----------
   10            metric     
   20            metric     
   20            metric     
   20            metric     

```

## show platform sand capabilities

```text
    Capability                              : Status
----------------------------------------------------
Sand:
-----
    Supported:
    ----------
    Maximum multicast groups                : 31744
    Maximum IP Security tunnel interfaces   : 0
    Maximum egress ARP table entries        : 32000
    Maximum SVI                             : 16000
    Maximum LAGs                            : 1024
    Usable LAGs                             : 1008
    Maximum software LAGs                   : 1152
    Maximum members per LAG                 : 16
    Maximum MAC table entries               : 65536
    LAG multicast load balancing
    Unsupported:
    ------------
    Sand DANZ runnable
    Sand IP security
    FEC for each hop

MSRP:
-----
    Supported:
    ----------
    MSRP

MVRP:
-----
    Supported:
    ----------
    MVRP

Routing:
--------
    Supported:
    ----------
    Tunnel interface modes                  : gre
    Maximum nexthop group ECMP              : 256
    Nexthop group MPLS label stack entries  : 12
    Nexthop group types                     : ipv6OverUdp
    Nexthop group types                     : ip
    Nexthop group types                     : gre
    Nexthop group types                     : mplsOverUdp
    Nexthop group types                     : mplsOverGre
    Nexthop group types                     : mpls
    Nexthop group types                     : ipv4OverUdp
    Maximum ECMP                            : 600
    VRF routing
    PBR
    PBR Nexthop Vrf
    IPv6 ACL PBR
    IPv6 nexthop PBR
    Nexthop group
    Nexthop group PBR
    MPLS match rule PBR
    Sflow DSCP rewrite
    URPF on all FAPs
    MPLS pseudowire
    MPLS static pseudowire
    MPLS VPNv4
    MPLS VPNv6

V6 Routing:
-----------
    Supported:
    ----------
    IPv6 Maximum ECMP                       : 600
    IPv6 ECMP

ARP:
----
    Supported:
    ----------
    ARP table size                          : 104448
    ARP neighbor table size                 : 208896

QoS:
----
    Supported:
    ----------
    Default CoS value                       : 0
    Default DSCP value                      : 0
    Minimum transmit queue shape rate       : 50000
    Minimum port shape rate                 : 1000
    Maximum shape rate (pps)                : 600000000
    Default CoS supported
    Default DSCP supported
    ECN
    WRED
    Hardware status reporting
    TC to DSCP map
    Dynamic Exp/TC mapping
    Unsupported:
    ------------
    Transmit queue shape rate unit (pps)

QoS ACL:
--------
    Supported:
    ----------
    Policy QoS actions                      : actionSetTc
    Policy QoS actions                      : actionSetDscp
    Number of QoS policy class maps         : 4096
    Police byte mode minimum burst bytes    : 0
    Police byte mode maximum burst bytes    : 4161500
    Police byte mode minimum rate (kbps)    : 1
    Police byte mode maximum rate (kbps)    : 1000000000
    Policy QoS
    Ingress policing
    Ingress trTcm (two rate three color) policing
    IPv4 ACLs
    IPv6 ACLs
    Shared policer
    QoS ACL asynchronous support required
    ACL hardware status reporting

Bridging:
---------
    Supported:
    ----------
    Dot1q tunnel
    VXLAN
    VXLAN BFD
    VXLAN L2 ECMP
    Unsupported:
    ------------
    VXLAN multicast group

Bridging/Topology:
------------------
    Supported:
    ----------
    Maximum topologies                      : 4095

Interfaces:
-----------
    Supported:
    ----------
    Congestion drops log direction          : directionTxAndRx

```

