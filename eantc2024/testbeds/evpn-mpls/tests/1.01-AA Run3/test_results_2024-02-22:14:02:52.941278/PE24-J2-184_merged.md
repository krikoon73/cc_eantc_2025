# Test results for PE24-J2-184

## show bgp evpn

```text
BGP routing table information for VRF default
Router identifier 100.0.0.184, local AS number 64512
Route status codes: * - valid, > - active, S - Stale, E - ECMP head, e - ECMP
                    c - Contributing to ECMP, % - Pending BGP convergence
Origin codes: i - IGP, e - EGP, ? - incomplete
AS Path Attributes: Or-ID - Originator ID, C-LST - Cluster List, LL Nexthop - Link Local Nexthop

          Network                Next Hop              Metric  LocPref Weight  Path
 * >Ec    RD: 100.0.0.56:4556 auto-discovery 56 0000:0000:0000:0000:0000
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
 *  ec    RD: 100.0.0.56:4556 auto-discovery 56 0000:0000:0000:0000:0000
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.3.58 
 * >Ec    RD: 100.0.0.56:2310 auto-discovery 2310 0000:0000:0000:0111:0111
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
 *  ec    RD: 100.0.0.56:2310 auto-discovery 2310 0000:0000:0000:0111:0111
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.3.58 
 * >Ec    RD: 100.0.0.181:2310 auto-discovery 2310 0000:0000:0000:0111:0111
                                 100.0.0.181           -       100     0       i Or-ID: 100.0.0.181 C-LST: 100.0.0.180 
 *  ec    RD: 100.0.0.181:2310 auto-discovery 2310 0000:0000:0000:0111:0111
                                 100.0.0.181           -       100     0       i Or-ID: 100.0.0.181 C-LST: 100.0.3.58 
 * >Ec    RD: 100.0.0.56:2310 auto-discovery 0000:0000:0000:0111:0111
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
 *  ec    RD: 100.0.0.56:2310 auto-discovery 0000:0000:0000:0111:0111
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.3.58 
 * >Ec    RD: 100.0.0.181:1 auto-discovery 0000:0000:0000:0111:0111
                                 100.0.0.181           -       100     0       i Or-ID: 100.0.0.181 C-LST: 100.0.0.180 
 *  ec    RD: 100.0.0.181:1 auto-discovery 0000:0000:0000:0111:0111
                                 100.0.0.181           -       100     0       i Or-ID: 100.0.0.181 C-LST: 100.0.3.58 
 * >Ec    RD: 100.0.0.183:2183 auto-discovery 0 0000:0000:0000:0183:0184
                                 100.0.0.183           -       100     0       i Or-ID: 100.0.0.183 C-LST: 100.0.0.180 
 *  ec    RD: 100.0.0.183:2183 auto-discovery 0 0000:0000:0000:0183:0184
                                 100.0.0.183           -       100     0       i Or-ID: 100.0.0.183 C-LST: 100.0.3.58 
 * >Ec    RD: 100.0.0.183:2301 auto-discovery 0 0000:0000:0000:0183:0184
                                 100.0.0.183           -       100     0       i Or-ID: 100.0.0.183 C-LST: 100.0.0.180 
 *  ec    RD: 100.0.0.183:2301 auto-discovery 0 0000:0000:0000:0183:0184
                                 100.0.0.183           -       100     0       i Or-ID: 100.0.0.183 C-LST: 100.0.3.58 
 * >Ec    RD: 100.0.0.183:2302 auto-discovery 0 0000:0000:0000:0183:0184
                                 100.0.0.183           -       100     0       i Or-ID: 100.0.0.183 C-LST: 100.0.0.180 
 *  ec    RD: 100.0.0.183:2302 auto-discovery 0 0000:0000:0000:0183:0184
                                 100.0.0.183           -       100     0       i Or-ID: 100.0.0.183 C-LST: 100.0.3.58 
 * >Ec    RD: 100.0.0.183:2303 auto-discovery 0 0000:0000:0000:0183:0184
                                 100.0.0.183           -       100     0       i Or-ID: 100.0.0.183 C-LST: 100.0.0.180 
 *  ec    RD: 100.0.0.183:2303 auto-discovery 0 0000:0000:0000:0183:0184
                                 100.0.0.183           -       100     0       i Or-ID: 100.0.0.183 C-LST: 100.0.3.58 
 * >      RD: 100.0.0.184:2183 auto-discovery 0 0000:0000:0000:0183:0184
                                 -                     -       -       0       i
 * >      RD: 100.0.0.184:2301 auto-discovery 0 0000:0000:0000:0183:0184
                                 -                     -       -       0       i
 * >      RD: 100.0.0.184:2302 auto-discovery 0 0000:0000:0000:0183:0184
                                 -                     -       -       0       i
 * >      RD: 100.0.0.184:2303 auto-discovery 0 0000:0000:0000:0183:0184
                                 -                     -       -       0       i
 * >Ec    RD: 100.0.0.183:1 auto-discovery 0000:0000:0000:0183:0184
                                 100.0.0.183           -       100     0       i Or-ID: 100.0.0.183 C-LST: 100.0.0.180 
 *  ec    RD: 100.0.0.183:1 auto-discovery 0000:0000:0000:0183:0184
                                 100.0.0.183           -       100     0       i Or-ID: 100.0.0.183 C-LST: 100.0.3.58 
 * >      RD: 100.0.0.184:1 auto-discovery 0000:0000:0000:0183:0184
                                 -                     -       -       0       i
 * >Ec    RD: 100.0.0.34:2310 auto-discovery 2311 0000:0000:0000:0222:0222
                                 100.0.0.34            -       100     0       i Or-ID: 100.0.0.34 C-LST: 100.0.0.180 
 *  ec    RD: 100.0.0.34:2310 auto-discovery 2311 0000:0000:0000:0222:0222
                                 100.0.0.34            -       100     0       i Or-ID: 100.0.0.34 C-LST: 100.0.3.58 
 * >Ec    RD: 100.0.3.45:2311 auto-discovery 2311 0000:0000:0000:0222:0222
                                 100.0.3.45            -       100     0       i Or-ID: 100.0.3.45 C-LST: 100.0.0.180 
 *  ec    RD: 100.0.3.45:2311 auto-discovery 2311 0000:0000:0000:0222:0222
                                 100.0.3.45            -       100     0       i Or-ID: 100.0.3.45 C-LST: 100.0.3.58 
 * >Ec    RD: 100.0.0.34:0 auto-discovery 0000:0000:0000:0222:0222
                                 100.0.0.34            -       100     0       i Or-ID: 100.0.0.34 C-LST: 100.0.0.180 
 *  ec    RD: 100.0.0.34:0 auto-discovery 0000:0000:0000:0222:0222
                                 100.0.0.34            -       100     0       i Or-ID: 100.0.0.34 C-LST: 100.0.3.58 
 * >Ec    RD: 100.0.3.48:4558 auto-discovery 0 0048:5648:5648:5648:5648
                                 100.0.3.48            -       100     0       i Or-ID: 100.0.3.48 C-LST: 100.0.0.180 
 *  ec    RD: 100.0.3.48:4558 auto-discovery 0 0048:5648:5648:5648:5648
                                 100.0.3.48            -       100     0       i Or-ID: 100.0.3.48 C-LST: 100.0.3.58 
 * >Ec    RD: 100.0.3.48:2320 auto-discovery 2320 0048:5648:5648:5648:5648
                                 100.0.3.48            -       100     0       i Or-ID: 100.0.3.48 C-LST: 100.0.0.180 
 *  ec    RD: 100.0.3.48:2320 auto-discovery 2320 0048:5648:5648:5648:5648
                                 100.0.3.48            -       100     0       i Or-ID: 100.0.3.48 C-LST: 100.0.3.58 
 * >Ec    RD: 100.0.3.48:2320 auto-discovery 2321 0048:5648:5648:5648:5648
                                 100.0.3.48            -       100     0       i Or-ID: 100.0.3.48 C-LST: 100.0.0.180 
 *  ec    RD: 100.0.3.48:2320 auto-discovery 2321 0048:5648:5648:5648:5648
                                 100.0.3.48            -       100     0       i Or-ID: 100.0.3.48 C-LST: 100.0.3.58 
 * >Ec    RD: 100.0.3.48:1 auto-discovery 0048:5648:5648:5648:5648
                                 100.0.3.48            -       100     0       i Or-ID: 100.0.3.48 C-LST: 100.0.0.180 
 *  ec    RD: 100.0.3.48:1 auto-discovery 0048:5648:5648:5648:5648
                                 100.0.3.48            -       100     0       i Or-ID: 100.0.3.48 C-LST: 100.0.3.58 
 * >Ec    RD: 100.0.0.56:2056 mac-ip 0056.5656.5656 20.10.56.253
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
 *  ec    RD: 100.0.0.56:2056 mac-ip 0056.5656.5656 20.10.56.253
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.3.58 
 * >Ec    RD: 100.0.0.56:2301 mac-ip 0056.5656.5656 20.30.1.254
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
 *  ec    RD: 100.0.0.56:2301 mac-ip 0056.5656.5656 20.30.1.254
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.3.58 
 * >Ec    RD: 100.0.0.56:2302 mac-ip 0056.5656.5656 20.30.2.254
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
 *  ec    RD: 100.0.0.56:2302 mac-ip 0056.5656.5656 20.30.2.254
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.3.58 
 * >Ec    RD: 100.0.0.56:2056 mac-ip 00aa.aaaa.aaaa 20.10.56.254
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
 *  ec    RD: 100.0.0.56:2056 mac-ip 00aa.aaaa.aaaa 20.10.56.254
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.3.58 
 * >Ec    RD: 100.0.0.56:2301 mac-ip 00aa.aaaa.aaaa 20.30.1.254
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
 *  ec    RD: 100.0.0.56:2301 mac-ip 00aa.aaaa.aaaa 20.30.1.254
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.3.58 
 * >Ec    RD: 100.0.0.56:2302 mac-ip 00aa.aaaa.aaaa 20.30.2.254
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
 *  ec    RD: 100.0.0.56:2302 mac-ip 00aa.aaaa.aaaa 20.30.2.254
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.3.58 
 * >Ec    RD: 100.0.0.56:1111 mac-ip 185b.0089.c36e 192.168.1.254
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
 *  ec    RD: 100.0.0.56:1111 mac-ip 185b.0089.c36e 192.168.1.254
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.3.58 
 * >Ec    RD: 100.0.3.48:4558 mac-ip ecc0.1842.9427
                                 100.0.3.48            -       100     0       i Or-ID: 100.0.3.48 C-LST: 100.0.0.180 
 *  ec    RD: 100.0.3.48:4558 mac-ip ecc0.1842.9427
                                 100.0.3.48            -       100     0       i Or-ID: 100.0.3.48 C-LST: 100.0.3.58 
 * >Ec    RD: 100.0.0.56:2303 mac-ip 2303 0056.5656.5656 20.30.3.254
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
 *  ec    RD: 100.0.0.56:2303 mac-ip 2303 0056.5656.5656 20.30.3.254
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.3.58 
 * >Ec    RD: 100.0.0.56:2303 mac-ip 2303 00aa.aaaa.aaaa 20.30.3.254
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
 *  ec    RD: 100.0.0.56:2303 mac-ip 2303 00aa.aaaa.aaaa 20.30.3.254
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.3.58 
 * >Ec    RD: 100.0.0.56:2304 mac-ip 2304 0056.5656.5656 20.30.4.254
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
 *  ec    RD: 100.0.0.56:2304 mac-ip 2304 0056.5656.5656 20.30.4.254
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.3.58 
 * >Ec    RD: 100.0.0.56:2304 mac-ip 2304 00aa.aaaa.aaaa 20.30.4.254
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
 *  ec    RD: 100.0.0.56:2304 mac-ip 2304 00aa.aaaa.aaaa 20.30.4.254
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.3.58 
 * >      RD: 2300:2300 imet 100.0.0.21
                                 100.0.0.21            0       100     0       i Or-ID: 100.0.0.21 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.26:2301 imet 100.0.0.26
                                 100.0.0.26            0       100     0       i Or-ID: 100.0.0.26 C-LST: 100.0.0.180 
 * >      RD: 100.0.0.26:2302 imet 100.0.0.26
                                 100.0.0.26            0       100     0       i Or-ID: 100.0.0.26 C-LST: 100.0.0.180 
 * >Ec    RD: 100.0.0.56:1111 imet 100.0.0.56
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
 *  ec    RD: 100.0.0.56:1111 imet 100.0.0.56
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.3.58 
 * >Ec    RD: 100.0.0.56:2056 imet 100.0.0.56
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
 *  ec    RD: 100.0.0.56:2056 imet 100.0.0.56
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.3.58 
 * >Ec    RD: 100.0.0.56:2301 imet 100.0.0.56
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
 *  ec    RD: 100.0.0.56:2301 imet 100.0.0.56
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.3.58 
 * >Ec    RD: 100.0.0.56:2302 imet 100.0.0.56
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
 *  ec    RD: 100.0.0.56:2302 imet 100.0.0.56
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.3.58 
 * >Ec    RD: 100.0.0.181:2181 imet 100.0.0.181
                                 100.0.0.181           -       100     0       i Or-ID: 100.0.0.181 C-LST: 100.0.0.180 
 *  ec    RD: 100.0.0.181:2181 imet 100.0.0.181
                                 100.0.0.181           -       100     0       i Or-ID: 100.0.0.181 C-LST: 100.0.3.58 
 * >Ec    RD: 100.0.0.181:2301 imet 100.0.0.181
                                 100.0.0.181           -       100     0       i Or-ID: 100.0.0.181 C-LST: 100.0.0.180 
 *  ec    RD: 100.0.0.181:2301 imet 100.0.0.181
                                 100.0.0.181           -       100     0       i Or-ID: 100.0.0.181 C-LST: 100.0.3.58 
 * >Ec    RD: 100.0.0.181:2302 imet 100.0.0.181
                                 100.0.0.181           -       100     0       i Or-ID: 100.0.0.181 C-LST: 100.0.0.180 
 *  ec    RD: 100.0.0.181:2302 imet 100.0.0.181
                                 100.0.0.181           -       100     0       i Or-ID: 100.0.0.181 C-LST: 100.0.3.58 
 * >Ec    RD: 100.0.0.182:2181 imet 100.0.0.182
                                 100.0.0.182           -       100     0       i Or-ID: 100.0.0.182 C-LST: 100.0.0.180 
 *  ec    RD: 100.0.0.182:2181 imet 100.0.0.182
                                 100.0.0.182           -       100     0       i Or-ID: 100.0.0.182 C-LST: 100.0.3.58 
 * >Ec    RD: 100.0.0.182:2301 imet 100.0.0.182
                                 100.0.0.182           -       100     0       i Or-ID: 100.0.0.182 C-LST: 100.0.0.180 
 *  ec    RD: 100.0.0.182:2301 imet 100.0.0.182
                                 100.0.0.182           -       100     0       i Or-ID: 100.0.0.182 C-LST: 100.0.3.58 
 * >Ec    RD: 100.0.0.182:2302 imet 100.0.0.182
                                 100.0.0.182           -       100     0       i Or-ID: 100.0.0.182 C-LST: 100.0.0.180 
 *  ec    RD: 100.0.0.182:2302 imet 100.0.0.182
                                 100.0.0.182           -       100     0       i Or-ID: 100.0.0.182 C-LST: 100.0.3.58 
 * >Ec    RD: 100.0.0.183:2183 imet 100.0.0.183
                                 100.0.0.183           -       100     0       i Or-ID: 100.0.0.183 C-LST: 100.0.0.180 
 *  ec    RD: 100.0.0.183:2183 imet 100.0.0.183
                                 100.0.0.183           -       100     0       i Or-ID: 100.0.0.183 C-LST: 100.0.3.58 
 * >Ec    RD: 100.0.0.183:2301 imet 100.0.0.183
                                 100.0.0.183           -       100     0       i Or-ID: 100.0.0.183 C-LST: 100.0.0.180 
 *  ec    RD: 100.0.0.183:2301 imet 100.0.0.183
                                 100.0.0.183           -       100     0       i Or-ID: 100.0.0.183 C-LST: 100.0.3.58 
 * >Ec    RD: 100.0.0.183:2302 imet 100.0.0.183
                                 100.0.0.183           -       100     0       i Or-ID: 100.0.0.183 C-LST: 100.0.0.180 
 *  ec    RD: 100.0.0.183:2302 imet 100.0.0.183
                                 100.0.0.183           -       100     0       i Or-ID: 100.0.0.183 C-LST: 100.0.3.58 
 * >      RD: 100.0.0.184:2183 imet 100.0.0.184
                                 -                     -       -       0       i
 * >      RD: 100.0.0.184:2301 imet 100.0.0.184
                                 -                     -       -       0       i
 * >      RD: 100.0.0.184:2302 imet 100.0.0.184
                                 -                     -       -       0       i
 * >Ec    RD: 100.0.3.48:4558 imet 100.0.3.48
                                 100.0.3.48            -       100     0       i Or-ID: 100.0.3.48 C-LST: 100.0.0.180 
 *  ec    RD: 100.0.3.48:4558 imet 100.0.3.48
                                 100.0.3.48            -       100     0       i Or-ID: 100.0.3.48 C-LST: 100.0.3.58 
 * >      RD: 100.0.0.26:2303 imet 2303 100.0.0.26
                                 100.0.0.26            0       100     0       i Or-ID: 100.0.0.26 C-LST: 100.0.0.180 
 * >Ec    RD: 100.0.0.56:2303 imet 2303 100.0.0.56
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
 *  ec    RD: 100.0.0.56:2303 imet 2303 100.0.0.56
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.3.58 
 * >Ec    RD: 100.0.0.181:2303 imet 2303 100.0.0.181
                                 100.0.0.181           -       100     0       i Or-ID: 100.0.0.181 C-LST: 100.0.0.180 
 *  ec    RD: 100.0.0.181:2303 imet 2303 100.0.0.181
                                 100.0.0.181           -       100     0       i Or-ID: 100.0.0.181 C-LST: 100.0.3.58 
 * >Ec    RD: 100.0.0.182:2303 imet 2303 100.0.0.182
                                 100.0.0.182           -       100     0       i Or-ID: 100.0.0.182 C-LST: 100.0.0.180 
 *  ec    RD: 100.0.0.182:2303 imet 2303 100.0.0.182
                                 100.0.0.182           -       100     0       i Or-ID: 100.0.0.182 C-LST: 100.0.3.58 
 * >Ec    RD: 100.0.0.183:2303 imet 2303 100.0.0.183
                                 100.0.0.183           -       100     0       i Or-ID: 100.0.0.183 C-LST: 100.0.0.180 
 *  ec    RD: 100.0.0.183:2303 imet 2303 100.0.0.183
                                 100.0.0.183           -       100     0       i Or-ID: 100.0.0.183 C-LST: 100.0.3.58 
 * >      RD: 100.0.0.184:2303 imet 2303 100.0.0.184
                                 -                     -       -       0       i
 * >      RD: 100.0.0.26:2304 imet 2304 100.0.0.26
                                 100.0.0.26            0       100     0       i Or-ID: 100.0.0.26 C-LST: 100.0.0.180 
 * >Ec    RD: 100.0.0.56:2304 imet 2304 100.0.0.56
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
 *  ec    RD: 100.0.0.56:2304 imet 2304 100.0.0.56
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.3.58 
 * >Ec    RD: 100.0.0.181:2303 imet 2304 100.0.0.181
                                 100.0.0.181           -       100     0       i Or-ID: 100.0.0.181 C-LST: 100.0.0.180 
 *  ec    RD: 100.0.0.181:2303 imet 2304 100.0.0.181
                                 100.0.0.181           -       100     0       i Or-ID: 100.0.0.181 C-LST: 100.0.3.58 
 * >Ec    RD: 100.0.0.182:2303 imet 2304 100.0.0.182
                                 100.0.0.182           -       100     0       i Or-ID: 100.0.0.182 C-LST: 100.0.0.180 
 *  ec    RD: 100.0.0.182:2303 imet 2304 100.0.0.182
                                 100.0.0.182           -       100     0       i Or-ID: 100.0.0.182 C-LST: 100.0.3.58 
 * >Ec    RD: 100.0.0.183:2303 imet 2304 100.0.0.183
                                 100.0.0.183           -       100     0       i Or-ID: 100.0.0.183 C-LST: 100.0.0.180 
 *  ec    RD: 100.0.0.183:2303 imet 2304 100.0.0.183
                                 100.0.0.183           -       100     0       i Or-ID: 100.0.0.183 C-LST: 100.0.3.58 
 * >      RD: 100.0.0.184:2303 imet 2304 100.0.0.184
                                 -                     -       -       0       i
 * >Ec    RD: 100.0.0.56:0 ethernet-segment 0000:0000:0000:0111:0111 100.0.0.56
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
 *  ec    RD: 100.0.0.56:0 ethernet-segment 0000:0000:0000:0111:0111 100.0.0.56
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.3.58 
 * >Ec    RD: 100.0.0.181:1 ethernet-segment 0000:0000:0000:0111:0111 100.0.0.181
                                 100.0.0.181           -       100     0       i Or-ID: 100.0.0.181 C-LST: 100.0.0.180 
 *  ec    RD: 100.0.0.181:1 ethernet-segment 0000:0000:0000:0111:0111 100.0.0.181
                                 100.0.0.181           -       100     0       i Or-ID: 100.0.0.181 C-LST: 100.0.3.58 
 * >Ec    RD: 100.0.0.183:1 ethernet-segment 0000:0000:0000:0183:0184 100.0.0.183
                                 100.0.0.183           -       100     0       i Or-ID: 100.0.0.183 C-LST: 100.0.0.180 
 *  ec    RD: 100.0.0.183:1 ethernet-segment 0000:0000:0000:0183:0184 100.0.0.183
                                 100.0.0.183           -       100     0       i Or-ID: 100.0.0.183 C-LST: 100.0.3.58 
 * >      RD: 100.0.0.184:1 ethernet-segment 0000:0000:0000:0183:0184 100.0.0.184
                                 -                     -       -       0       i
 * >Ec    RD: 100.0.0.34:0 ethernet-segment 0000:0000:0000:0222:0222 100.0.0.34
                                 100.0.0.34            -       100     0       i Or-ID: 100.0.0.34 C-LST: 100.0.0.180 
 *  ec    RD: 100.0.0.34:0 ethernet-segment 0000:0000:0000:0222:0222 100.0.0.34
                                 100.0.0.34            -       100     0       i Or-ID: 100.0.0.34 C-LST: 100.0.3.58 
 * >Ec    RD: 100.0.3.48:0 ethernet-segment 0048:5648:5648:5648:5648 100.0.3.48
                                 100.0.3.48            -       100     0       i Or-ID: 100.0.3.48 C-LST: 100.0.0.180 
 *  ec    RD: 100.0.3.48:0 ethernet-segment 0048:5648:5648:5648:5648 100.0.3.48
                                 100.0.3.48            -       100     0       i Or-ID: 100.0.3.48 C-LST: 100.0.3.58 
 * >      RD: 100.0.0.184:2000 ip-prefix 10.30.4.0/24
                                 -                     -       -       0       i
 * >Ec    RD: 100.0.0.56:2000 ip-prefix 20.10.56.0/24
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
 *  ec    RD: 100.0.0.56:2000 ip-prefix 20.10.56.0/24
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.3.58 
 * >Ec    RD: 100.0.0.183:2000 ip-prefix 20.10.183.0/24
                                 100.0.0.183           -       100     0       i Or-ID: 100.0.0.183 C-LST: 100.0.0.180 
 *  ec    RD: 100.0.0.183:2000 ip-prefix 20.10.183.0/24
                                 100.0.0.183           -       100     0       i Or-ID: 100.0.0.183 C-LST: 100.0.3.58 
 * >      RD: 100.0.0.184:2000 ip-prefix 20.10.183.0/24
                                 -                     -       -       0       i
 * >      RD: 2301:2301 ip-prefix 20.30.1.0/24
                                 100.0.0.21            0       100     0       i Or-ID: 100.0.0.21 C-LST: 100.0.0.180 
 * >Ec    RD: 100.0.0.56:2000 ip-prefix 20.30.1.0/24
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
 *  ec    RD: 100.0.0.56:2000 ip-prefix 20.30.1.0/24
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.3.58 
 * >Ec    RD: 100.0.0.183:2000 ip-prefix 20.30.1.0/24
                                 100.0.0.183           -       100     0       i Or-ID: 100.0.0.183 C-LST: 100.0.0.180 
 *  ec    RD: 100.0.0.183:2000 ip-prefix 20.30.1.0/24
                                 100.0.0.183           -       100     0       i Or-ID: 100.0.0.183 C-LST: 100.0.3.58 
 * >      RD: 100.0.0.184:2000 ip-prefix 20.30.1.0/24
                                 -                     -       -       0       i
 * >Ec    RD: 100.0.0.56:2000 ip-prefix 20.30.2.0/24
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
 *  ec    RD: 100.0.0.56:2000 ip-prefix 20.30.2.0/24
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.3.58 
 * >Ec    RD: 100.0.0.183:2000 ip-prefix 20.30.2.0/24
                                 100.0.0.183           -       100     0       i Or-ID: 100.0.0.183 C-LST: 100.0.0.180 
 *  ec    RD: 100.0.0.183:2000 ip-prefix 20.30.2.0/24
                                 100.0.0.183           -       100     0       i Or-ID: 100.0.0.183 C-LST: 100.0.3.58 
 * >      RD: 100.0.0.184:2000 ip-prefix 20.30.2.0/24
                                 -                     -       -       0       i
 * >Ec    RD: 100.0.0.56:2000 ip-prefix 20.30.3.0/24
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
 *  ec    RD: 100.0.0.56:2000 ip-prefix 20.30.3.0/24
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.3.58 
 * >Ec    RD: 100.0.0.183:2000 ip-prefix 20.30.3.0/24
                                 100.0.0.183           -       100     0       i Or-ID: 100.0.0.183 C-LST: 100.0.0.180 
 *  ec    RD: 100.0.0.183:2000 ip-prefix 20.30.3.0/24
                                 100.0.0.183           -       100     0       i Or-ID: 100.0.0.183 C-LST: 100.0.3.58 
 * >      RD: 100.0.0.184:2000 ip-prefix 20.30.3.0/24
                                 -                     -       -       0       i
 * >Ec    RD: 100.0.0.56:2000 ip-prefix 20.30.4.0/24
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
 *  ec    RD: 100.0.0.56:2000 ip-prefix 20.30.4.0/24
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.3.58 
 * >Ec    RD: 100.0.0.183:2000 ip-prefix 20.30.4.0/24
                                 100.0.0.183           -       100     0       i Or-ID: 100.0.0.183 C-LST: 100.0.0.180 
 *  ec    RD: 100.0.0.183:2000 ip-prefix 20.30.4.0/24
                                 100.0.0.183           -       100     0       i Or-ID: 100.0.0.183 C-LST: 100.0.3.58 
 * >Ec    RD: 100.0.0.31:7 ip-prefix 31.31.31.31/32
                                 100.0.0.31            -       100     0       i Or-ID: 100.0.0.31 C-LST: 100.0.0.180 
 *  ec    RD: 100.0.0.31:7 ip-prefix 31.31.31.31/32
                                 100.0.0.31            -       100     0       i Or-ID: 100.0.0.31 C-LST: 100.0.3.58 
 * >Ec    RD: 100.0.0.56:100 ip-prefix 56.56.56.56/32
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
 *  ec    RD: 100.0.0.56:100 ip-prefix 56.56.56.56/32
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.3.58 
 * >Ec    RD: 100.0.0.56:1111 ip-prefix 56.56.56.56/32
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
 *  ec    RD: 100.0.0.56:1111 ip-prefix 56.56.56.56/32
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.3.58 
 * >Ec    RD: 100.0.0.56:100 ip-prefix 192.168.1.0/24
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.0.180 
 *  ec    RD: 100.0.0.56:100 ip-prefix 192.168.1.0/24
                                 100.0.0.56            -       100     0       i Or-ID: 100.0.0.56 C-LST: 100.0.3.58 
 * >Ec    RD: 100.0.3.48:4558 smet (S, G): (*, 239.0.0.100) originating IP: 100.0.3.48
                                 100.0.3.48            -       100     0       i Or-ID: 100.0.3.48 C-LST: 100.0.0.180 
 *  ec    RD: 100.0.3.48:4558 smet (S, G): (*, 239.0.0.100) originating IP: 100.0.3.48
                                 100.0.3.48            -       100     0       i Or-ID: 100.0.3.48 C-LST: 100.0.3.58 
 * >Ec    RD: 100.0.3.48:4558 join-sync ETID: 10 ESI: 0048:5648:5648:5648:5648 (S, G): (*, 239.0.0.100) originating IP: 100.0.3.48
                                 100.0.3.48            -       100     0       i Or-ID: 100.0.3.48 C-LST: 100.0.0.180 
 *  ec    RD: 100.0.3.48:4558 join-sync ETID: 10 ESI: 0048:5648:5648:5648:5648 (S, G): (*, 239.0.0.100) originating IP: 100.0.3.48
                                 100.0.3.48            -       100     0       i Or-ID: 100.0.3.48 C-LST: 100.0.3.58 
```

## show bgp evpn instance

```text
EVPN instance: VLAN 2183
  Route distinguisher: 100.0.0.184:2183
  Route target import: Route-Target-AS:2183:2183
  Route target export: Route-Target-AS:2183:2183
  Service interface: VLAN-based
  Local MPLS IP address: 100.0.0.184
  VXLAN: disabled
  MPLS: enabled
  Label allocation mode: per-instance
  MAC route MPLS label: 1046830
  IMET route MPLS label: 1039673
  AD route MPLS label: 1046830
  Local ethernet segment:
    ESI: 0000:0000:0000:0183:0184
      Interface: Port-Channel200
      Mode: all-active
      State: up
      ESI label: 1036288
      ES-Import RT: 00:00:18:30:01:84
      DF election algorithm: preference
      Designated forwarder: 100.0.0.183
      Non-Designated forwarder: 100.0.0.184
EVPN instance: VLAN 2301
  Route distinguisher: 100.0.0.184:2301
  Route target import: Route-Target-AS:2301:2301
  Route target export: Route-Target-AS:2301:2301
  Service interface: VLAN-based
  Local MPLS IP address: 100.0.0.184
  VXLAN: disabled
  MPLS: enabled
  Label allocation mode: per-instance
  MAC route MPLS label: 1036801
  IMET route MPLS label: 1039671
  AD route MPLS label: 1036801
  Local ethernet segment:
    ESI: 0000:0000:0000:0183:0184
      Interface: Port-Channel200
      Mode: all-active
      State: up
      ESI label: 1036288
      ES-Import RT: 00:00:18:30:01:84
      DF election algorithm: preference
      Designated forwarder: 100.0.0.183
      Non-Designated forwarder: 100.0.0.184
EVPN instance: VLAN 2302
  Route distinguisher: 100.0.0.184:2302
  Route target import: Route-Target-AS:2302:2302
  Route target export: Route-Target-AS:2302:2302
  Service interface: VLAN-based
  Local MPLS IP address: 100.0.0.184
  VXLAN: disabled
  MPLS: enabled
  Label allocation mode: per-instance
  MAC route MPLS label: 1042979
  IMET route MPLS label: 1038234
  AD route MPLS label: 1042979
  Local ethernet segment:
    ESI: 0000:0000:0000:0183:0184
      Interface: Port-Channel200
      Mode: all-active
      State: up
      ESI label: 1036288
      ES-Import RT: 00:00:18:30:01:84
      DF election algorithm: preference
      Designated forwarder: 100.0.0.183
      Non-Designated forwarder: 100.0.0.184
EVPN instance: VLAN-aware bundle 2303-2304
  Route distinguisher: 100.0.0.184:2303
  Route target import: Route-Target-AS:2303:2303
  Route target export: Route-Target-AS:2303:2303
  Service interface: VLAN-aware bundle
  Local MPLS IP address: 100.0.0.184
  VXLAN: disabled
  MPLS: enabled
  Label allocation mode: per-instance
  MAC route MPLS label: 1040269
  IMET route MPLS label: 1046862
  AD route MPLS label: 1040269
  Local ethernet segment:
    ESI: 0000:0000:0000:0183:0184
      Interface: Port-Channel200
      Mode: all-active
      State: up
      ESI label: 1036288
      ES-Import RT: 00:00:18:30:01:84
      DF election algorithm: preference
      Designated forwarder: 100.0.0.183
      Non-Designated forwarder: 100.0.0.184
```

## show patch panel

```text
Patch Connector Status Last Change
----- --------- ------ -----------

```

## show version

```text
Arista DCS-7280SR3-40YC6-F
Hardware version: 11.02
Serial number: SGD231508WS
Hardware MAC address: c4ca.2b45.e739
System MAC address: c4ca.2b45.e739

Software image version: 4.28.6.1M
Architecture: i686
Internal build version: 4.28.6.1M-30820457.42861M
Internal build ID: 6064e036-b8b7-433c-8425-5e378eaa9915
Image format version: 3.0
Image optimization: Default

Uptime: 3 days, 7 hours and 9 minutes
Total memory: 8147100 kB
Free memory: 5761744 kB

```

