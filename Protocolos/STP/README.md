STP
=========


**MSTP_Intra-Region_BPDUs.cap** de http://packetlife.net/

Descripción original:
MSTP BPDUs captured on an intra-region root port.
00:1f:27:b4:7d:80 - CIST Root (is in another MSTP Region)
00:16:46:b5:8c:80 - CIST Regional Root, Root for Instance 0, 2
00:1e:f7:05:a8:80 - Root for Instance 1
Notice in frame 1 that 00:1e:f7:05:a8:80 uses 32768.00:16:46:b5:8c:80 (Regional Root BID) as bridge ID in the main STP header to make the region appear as a single bridge.

**packet-c.cap** de http://packetlife.net/

Descripción original:
Packets: 926	Duration: 13s	Downloads: 6974
This is a packet capture from a SonicWall. We were troubleshooting DHCP packet flows. The SonicWall saw the DHCP Discover and Sent an Offer. We never saw the DHCP acknowledgement. In the adjacent core stacked switching we were running "debug ip dhcp server packets" we only saw discover packets from IP phones up to the SonicWall. For some reason the SonicWall could not let any other DHCP packets through or out of it INSIDE (LAN) interface. Even if we put an ANY-ANY ALC for that interface. We ended up having to replace the SonicWall and upload the configuration from the old SonicWall to the new one.
-Slaingod


**rpvstp-trunk-native-vid5.pcap.cap** de http://packetlife.net/

Descripción original:
Rapid per-VLAN spanning tree capture of a trunk port, configured with native VLAN 5, VLAN 1 is also active over the trunk.
Capture shows that 3 BPDUs are sent out, one for classic STP (Frame 4, for example), one for the native VLAN 5 (not tagged - Frame 5) and one for each other active VLAN (tagged - Frame 3).
The PVST BPDUs contain the VLAN ID at the end of the frame (01 and 05, respectively).

**rpvstp-trunk-native-vid1.pcap.cap** de http://packetlife.net/

Descripción original:
Rapid per-VLAN spanning tree capture of a trunk port, configured with native VLAN 1 (default), VLAN 5 is also active over the trunk.
Capture shows that 3 BPDUs are sent out, one for classic STP (Frame 4, for example), one for the native VLAN (not tagged - Frame 3) and one for each other active VLAN (tagged - Frame 5).
The PVST BPDUs contain the VLAN ID at the end of the frame (01 and 05, respectively).

**rpvstp-access.pcap.cap** de http://packetlife.net/

Descripción original:
Rapid per-VLAN spanning tree capture of an access port (without portfast), configured in VLAN 5.

**802.1w_rapid_STP.cap** de http://packetlife.net/

Descripción original:
Rapid Spanning Tree Protocol BPDUs are received from a Catalyst switch after connecting to a port not configured for PortFast. The port transitions through the blocking and learning states before issuing a topology change notification (packet #30) and transitioning to the forwarding state.

**802.1D_spanning_tree.cap** de http://packetlife.net/

Descripción original:
IEEE 802.1D Spanning Tree Protocol (STP) advertisements sent every two seconds.
