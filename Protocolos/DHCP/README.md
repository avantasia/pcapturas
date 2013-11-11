DHCP
=========


**DHCP.cap** de http://packetlife.net/

Descripción original:
R0 is the client and R1 is the DHCP server. Lease time is 1 minute.

**DHCP_Inter_VLAN.cap** de http://packetlife.net/

Descripción original:
R1 is a router-on-a-stick. It receives a DHCP Discover on the trunk interface, it sets the "Relay agent IP address" to the sub-interface's IP address it received the packet on and, finally, it forwards it to the DHCP server. Capture perspective is R1-DHCP server link.

**DHCP_MessageType 10,11,12 and 13.cap** de http://packetlife.net/

Descripción original:
Access Concentrator/router queries lease for particular IP addresses using message type as "DHCP LEASE QUERY" and gets response as DHCP LEASE ACTIVE,LEASE UNASSIGNED and LEASE UNKNOWN.
Access Concenttrator/Router IP=10.10.39.14
DHCP server IP=10.10.35.33

