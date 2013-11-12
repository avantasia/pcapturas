ICMP
=========
**icmp**, **destunreachable** y **icmp-tracert-slow** de "Practical Packet Analysis - Using Wireshark to Solve Real-World Network Problems" - Chris Sanders

**icmp** **fragmented** de http://packetlife.net/

Descripción original:
pinged google.com with -l option in windows which allows us to set the data size of the packet.
Data size of 15000 bytes has been chosen and we can see that it is fragmented through the network into a maximum data size 1480 bytes in each packet.
We can also see offset and identification field set in the ip header.

**icmp with record route option set.cap** de http://packetlife.net/

Descripción original:
ping packet with record route option set and IP addresses of all outgoing and incoming interfaces along the path.
In that we can also see position of current pointer.

**traceroute_MPLS.cap** de http://packetlife.net/

PPP.cap de http://packetlife.net/
Descripción original:
ICMP across a PPP serial link.

**path_MTU_discovery.cap** de http://packetlife.net/

Descripción original:
Tracepath is used to determine the MTU of the path between hosts 192.168.0.2 and .1.2. Packet #6 contains an ICMP "fragmentation needed" message, indicating the MTU for that hop is 1400 bytes.

**MPLS_encapsulation.cap** de http://packetlife.net/

Descripción original:
Capture taken from the PE1-P1 link. ICMP traffic between CE1 and CE2 is encapsulated outbound with MPLS label 18. Note that returning traffic is not labeled, due to penultimate hop popping (PHP).

**ICMP_across_frame_relay.cap** de http://packetlife.net/

Descripción original:
A Cisco 3725 pinging its neighbor across a point-to-point frame relay connection.

**ICMP_across_dot1q.cap** de http://packetlife.net/

Descripción original:
A ping issued from 192.168.123.2 to 192.168.123.1 is encapsulated with an IEEE 802.1Q header, placing it in VLAN 123.

**HDLC.cap** de http://packetlife.net/

Descripción original:
ICMP across an HDLC serial link.



