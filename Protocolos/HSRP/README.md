HSRP
=========

HSRP_failover.cap de http://packetlife.net/
Descripción original:
R1 is the active router, R3 is the standby, and R2 is passive. R1 goes offline and R3 takes over as active after ten seconds. R2 is then promoted to the standby state.


HSRP_election.cap de http://packetlife.net/
Descripción original:
The Ethernet link shared by routers 1, 2, and 3 comes online. R1 wins the HSRP election because it has a priority of 200 (versus the default of 100 held by the other two routers). R3 becomes the standby router.

HSRP_coup.cap de http://packetlife.net/
Descripción original:
Initially only routers 3 (active) and 2 (standby) are online. R1 comes online with a priority higher than R3's. R1 takes over as the active router (the coup occurs in packet #22) almost immediately. R2 is bumped down to passive and R3 becomes the standby router.
