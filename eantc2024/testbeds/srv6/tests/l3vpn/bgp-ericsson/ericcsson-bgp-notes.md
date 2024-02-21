# DT46 not supported

Ericsson only supports DT46, that is not accepted by our switches.
Node ID - 49
Example subnet: 20.49.225.0/24

```text
	Update Message (2), length: 157
	  Multi-Protocol Reach NLRI (14), length: 44, Flags [OE]:
	    AFI: IPv4 (1), SAFI: labeled VPN Unicast (128)
	    nexthop: RD: 0:0 (= 0.0.0.0), 32.2.0.0, RD: 0:0 (= 0.0.0.0), 0.0.0.73, nh-length: 24, no SNPA
	      RD: 1:49 (= 0.0.0.49), 20.49.225.0/24, label:3 (bottom)
	    0x0000:  0001 8018 0000 0000 0000 0000 2002 0000
	    0x0010:  0000 0000 0000 0000 0000 0049 0070 0000
	    0x0020:  3100 0000 0100 0000 3114 31e1
	  Origin (1), length: 1, Flags [T]: Incomplete
	    0x0000:  02
	  AS Path (2), length: 0, Flags [T]: empty
	  Multi Exit Discriminator (4), length: 4, Flags [O]: 0
	    0x0000:  0000 0000
	  Local Preference (5), length: 4, Flags [T]: 100
	    0x0000:  0000 0064
	  Extended Community (16), length: 8, Flags [OT]:
	    target (0x0002), Flags [none]: 1:20 (= 0.0.0.20)
	    0x0000:  0002 0001 0000 0014
	  Cluster List (10), length: 4, Flags [O]: pool-100-0-0-53.bstnma.fios.verizon.net
	    0x0000:  6400 0035
	  Originator ID (9), length: 4, Flags [O]: 10.0.0.49
	    0x0000:  0a00 0031
	  Unknown Attribute (40), length: 37, Flags [OT]:
	    no Attribute 40 decoder
	    0x0000:  0500 2200 0100 1e00 fcbb 0000 1049 e000
	    0x0010:  0000 0000 0000 0000 0000 4000 0100 0620
	    0x0020:  1010 0000 00
```
