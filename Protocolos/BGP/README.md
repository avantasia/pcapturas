BGP
=========

**BGP_MP_NLRI** de http://packetlife.net/

Descripción original:
IPv6 routes are carried as a separate address family inside MP_REACH_NLRI attributes.


**4-byte_AS_numbers_Mixed_Scenario** de http://packetlife.net/

Descripción original:
Router "B" (AS 2) at 172.16.3.2 does not support 4-byte AS numbers, while router "A" (AS 10.1 / 655361) at 172.16.3.1 does.
Router "A" receives an UPDATE for the 40.0.0.0/8 subnet from an external router ("D") in the AS 40.1 / 2621441 (not shown), and it forwards it to "B" (pkt n. 2): AS_PATH contains "23456 23456" (the first stands for AS 10.1, the second for the originating AS 40.1), but NEW_AS_PATH contains the real 4-byte AS numbers.
At pkt n. 3 "B" receives the same subnet directly from "D" and sends it to "A", including the original NEW_AS_PATH attribute previously appended by "D".

**4-byte_AS_numbers_Full_Support** de http://packetlife.net/

Descripción original:
Router at 172.16.1.2 (hostname "D", AS 40.1 / 2621441) clears a previous established peering with 172.16.1.1 (hostname "A", AS 10.1 / 655361); They both support 32-bit ASN.
While opening the new session, they negotiate the "Four-octet AS Number Capability" (pkts n. 2 and 3).
Then, both "A" and "D" send some UPDATEs containing 4-octect encoded AS_PATH attributes (pkts n. 6 and 9). Please note: WireShark may show wrong paths unless you force 4-byte encoding in the Preferences / Protocols / BGP options.

**BGP_MD5** de http://packetlife.net/

Descripción original:
An EBGP with TCP MD5 authentication enabled

**BGP_redist** de http://packetlife.net/

Descripción original:
The OSPF metric is preserved and propagated within the MPLS cloud by the MP-BGP MED attribute.

**IBGP_adjacency** de http://packetlife.net/

Descripción original:
Routers 3 and 4 form an internal BGP relationship. This is evidenced by the OPEN messages in packets #4 and #5, which show both routers belong to the same AS (65300). Also note that IBGP packets are not subject to a limited TTL as are EBGP packets.

**EBGP_adjacency** de http://packetlife.net/

Descripción original:
The external BGP adjacency between routers 1 and 2 is brought online and routes are exchanged. Keepalives are then exchanged every 60 seconds. Note that the IP TTL (normally 1) has been increased to 2 with ebgp-multihop to facilitate communication between the routers' loopback interfaces.

**BGP_soft_reset** de http://packetlife.net/

Descripción original:
R1 performs a soft bidirectional reset (clear ip bgp soft) on its adjacency with R2. The ROUTE-REFRESH message is visible in packet #7. Note that the TCP connection remains uninterrupted, and neither router views the reset as disruptive.

**BGP_notification** de http://packetlife.net/

Descripción original:
R1 has been misconfigured to expect R2 to reside in AS 65100. R2 attempts to peer with R1 advertising itself correctly in AS 65200. R1 issues a NOTIFICATION in packet #5 citing a "bad peer AS" error and terminates the TCP connection.

**BGP_hard_reset** de http://packetlife.net/

Descripción original:
A hard reset (clear ip bgp) is performed on R1 for its adjacency with R2. Packet #7 shows R1 sending a packet with the TCP FIN flag set, indicating the connection is to be torn down. The TCP connection is then reestablished and UPDATEs are retransmitted.

**BGP_AS_set** de http://packetlife.net/

Descripción original:
Packet #15 includes a BGP update containing both an AS sequence and an AS set in its AS path attribute.





