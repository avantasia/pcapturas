IGMP
=========


**IGMP_V1.cap** de http://packetlife.net/

Descripción original:
All IGMP V1 requests : Query General, Join specific group


**IGMP_V2.cap** de http://packetlife.net/

Descripción original:
All IGMP V2 requests : Query General, Query specfic group, Join specific group, leave specific group


**iphttps.cap** de http://packetlife.net/

Descripción original:
IP-HTTPS capture. This is Microsoft's IPv6 inside HTTPS tunneling for DirectAccess.


**PIM-SM_join_prune.cap** de http://packetlife.net/

Descripción original:
A host on R4's 172.16.20.0/24 subnet requests to join the 239.123.123.123 group. R4 sends a PIMv2 join message up to the RP (R1). Subsequent join messages are sent every 30 seconds, until R4 determines it no longer has any interested hosts and sends a prune request (packet #45). PIMv1 RP-Reachable messages for the group are also visible from R1.


**mtrace.cap** de http://packetlife.net/

Descripción original:
mtrace 172.16.40.1 172.16.20.1 is issued on R1 to trace the RPF path from R4's 172.16.20.0/24 subnet to R1's 172.16.40.0/24 subnet. The capture is taken on the R1-R3 link.


**mrinfo_query.cap **de http://packetlife.net/

Descripción original:
mrinfo 2.2.2.2 is issued on R1. DVMRPv3 is used to query R2 for its multicast interfaces.


**IGMPv2_query_and_report.cap** de http://packetlife.net/

Descripción original:
R1 issues IGMPv2 general membership queries to the 172.16.40.0/24 segment every 60 seconds. A host replies to each query reporting it belongs to the multicast group 239.255.255.250.




