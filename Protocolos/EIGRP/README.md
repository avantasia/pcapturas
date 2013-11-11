EIGRP
=========

**EIGRP_subnet_up** de http://packetlife.net/

Descripción original:
R4's 192.168.4.0/24 subnet is brought online. R1 receives updates from both R2 and R3 (only R2's update is shown in the capture). The poison-reverse in packet #9 informs R2 not to use R1 as a path to 192.168.4.0/24. The capture perspective is from R1's 10.0.0.1 interface.

**EIGRP_subnet_down** de http://packetlife.net/

Descripción original:
R4's interface to 192.168.4.0/24 goes down and the route is advertised as unreachable. Queries are issued by all routers to find a new path to the subnet but none exists, and the route is removed from the topology. Capture perspective is from R1's 10.0.0.1 interface.

**EIGRP_goodbye.cap** de http://packetlife.net/

Descripción original:
R2 designates its interface facing R1 as passive. The final hello message from R2 (packet #9) has all its K values set to 255, designating the message as a "goodbye." Capture perspective is from R1's 10.0.0.1 interface.

**EIGRP_adjacency.capde** http://packetlife.net/

Descripción original:
Formation of an EIGRP adjacency between routers R1 and R2. Capture point is R1's 10.0.0.1 interface.

**EIGRPv2_subnet_transition.cap** de http://packetlife.net/

Descripción original:
R4's 2001:db8:0:400::/64 subnet goes down, then comes back up roughly thirty seconds later. Capture perspective from R1's 2001:db8:0:12::1 interface.

**EIGRPv2_adjacency.cap** de http://packetlife.net/

Descripción original:
Routers 1 and 2 form an EIGRPv2 adjacency and exchange IPv6 routes.

