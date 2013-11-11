PIM
=========

**PIM_register_register-stop.cap** de http://packetlife.net/

Descripción original:
Switch at 192.168.0.6 receives an IGMP request for the group 239.1.2.3, encapsulates the original IGMP packet in a PIM Register and sends it to the RP at 192.168.1.254. In packet #2 RP sends a Register-Stop to the switch.

**PIMv2_hellos.cap** de http://packetlife.net/

Descripción original:
Routers 1 and 2 exchange PIMv2 hello packets.

**PIMv2_bootstrap.cap** de http://packetlife.net/

Descripción original:
Router 1 is the BSR and routers 2 and 3 are candidate RPs with the default priority of 0. R1 collects the RP advertisement unicasts from R2 and R3 and combines them in a bootstrap multicast to all PIM routers. Capture perspective is the R1-R3 link.

**PIM-SM_join_prune.cap** de http://packetlife.net/

Descripción original:
A host on R4's 172.16.20.0/24 subnet requests to join the 239.123.123.123 group. R4 sends a PIMv2 join message up to the RP (R1). Subsequent join messages are sent every 30 seconds, until R4 determines it no longer has any interested hosts and sends a prune request (packet #45). PIMv1 RP-Reachable messages for the group are also visible from R1.

**PIM-DM_pruning.cap** de http://packetlife.net/

Descripción original:
The multicast source at 172.16.40.10 begins sending traffic to the group 239.123.123.123, and PIM-DM floods the traffic down the tree. R4 has no group members, and prunes itself from the tree. R2 and R3 then realize they have no members, and each prunes itself from the tree. The capture shows R2 receiving the multicast traffic flooded from R1 and subsequently pruning itself every three minutes.