OSPF
=========

**ospf over gre tunnel.cap** de http://packetlife.net/

Descripción original:
Configured ospf over GRE tunnel in which packets are double tagged with ip header, useful when there is no direct connection between the 2 routers but still we need to run ospf.

**ospf simple password authentication.cap** de http://packetlife.net/

Descripción original:
Simple password authentication in ospf in which we can see password in clear text.
Also the auth type is also specified in the packet which is simple password.
I have also found a very interesting article regarding md5 auth mistakes made by many network engineers the link of which is below.
http://packetlife.net/blog/2010/jun/1/ospfv2-authentication-confusion/

**ICMP_over_L2TPv3_Pseudowire.pcap.cap** de http://packetlife.net/

Descripción original:
ICMP pings from a CE to a second CE via a L2TPv3 pseudowire.

**OSPF_Down-Bit.cap** de http://packetlife.net/

Descripción original:
LSA Update with down bit set. Router R5 56.0.0.5 PE is receiving an update from the MPLS VPN, which is advertised to CE 56.0.0.6 ospf routing table. In order for for the packet(LSA) not to be re-advertised back into the MPLS cloud through another PE(2) router, PE sets the Down-bit to 1. filter: ospf.v2.options.dn == 1

**OSPF_with_MD5_auth.cap** de http://packetlife.net/

Descripción original:
An OSPF adjacency is formed between two routers configured to use MD5 authentication.

**OSPF_type7_LSA.cap** de http://packetlife.net/

Descripción original:
Area 10 is configured as a not-so-stubby area (NSSA). The capture records the adjacency formed between routers 2 and 3. The link state update in packet #11 includes several type 7 LSAs from R2. Capture perspective from R3's 10.0.10.1 interface.

**OSPF_point-to-point_adjacencies.cap** de http://packetlife.net/

Descripción original:
The frame relay network between four routers is configured with point-to-point subinterfaces. No DR/BDR is required as all adjacencies are point-to-point. Capture perspective from R1.

**OSPF_NBMA_adjacencies.cap** de http://packetlife.net/

Descripción original:
Formation of OSPF adjacencies across a Non-broadcast Multiaccess (NBMA) frame relay topology. Neighbors have been manually specified on all routers, with R1 configured to become the DR. No BDR is present. Capture perspective from R1.

**OSPF_multipoint_adjacencies.cap** de http://packetlife.net/

Descripción original:
Routers 1 through 4 are configured to view the non-broadcast frame relay network as a point-to-multipoint topology. Adjacencies are formed without the need of a DR or BDR. Note that inverse ARP was used to dynamically learn the addresses of neighbors.


**OSPF_LSA_types.cap** de http://packetlife.net/

Descripción original:
Capture of adjacency formation between OSPF routers 4 and 5 in area 20. Packet #12 contains LSAs of types 1, 2, 3, 4, and 5.

**OSPF_broadcast_adjacencies.cap** de http://packetlife.net/

Descripción original:
Three routers form OSPF adjacencies across a broadcast segment. All interface priorities are left default, so R3 (with the highest router ID) becomes the DR, and R2 (with the next-highest router ID) becomes the BDR. Capture perspective from R1.

**OSPFv3_with_AH.cap** de http://packetlife.net/

Descripción original:
The adjacency between R1 and R2 in the 2001:db8:0:12::/64 subnet is configured with IPsec AH authentication. Note the inclusion of an IPsec AH header immediately following the IPv6 header of each OSPF packet.

**OSPFv3_NBMA_adjacencies.cap** de http://packetlife.net/

Descripción original:
Router 3 forms OSPFv3 adjacencies with routers 1 and two across the non-broadcast multi-access (NBMA) frame relay link.

**OSPFv3_multipoint_adjacencies.cap** de http://packetlife.net/

Descripción original:
The frame relay link connecting routers 1, 2, and 3 has been configured as a point-to-multipoint network with broadcast capability. Router 3 forms OSPFv3 adjacencies with routers 1 and 2, but no DR or BDR is elected.

**OSPFv3_broadcast_adjacency.cap** de http://packetlife.net/

Descripción original:
Routers 1 and 2 form an OSPFv3 adjacency across their common Ethernet link (2001:db8:0:12::/64).