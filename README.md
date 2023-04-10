# Datasets 5G-enabled Vehicular Networks

We use the NS-3 network simulator, which is open-source. We used the 5G-LENA module (<a href="https://gitlab.com/cttc-lena/nr">https://gitlab.com/cttc-lena/nr</a>), i.e., a GPLv2 New Radio (NR) network, called nr, that also allows to simulate 4G and 5G networks and V2X-based 5G communication. The simulator allows simulating some network actors, such as remote hosts that can connect to Packet Gateway and Service Gateway through a link and send it to gNodeB, and user equipment (i.e., vehicles). Additionally, the nr module is described as a “hard fork” of the millimeter-wave (mmWave) simulator, which enables simulating the physical (PHY) layer and medium access control (MAC), mmWave channel, propagation, beamforming, and antenna models.

The simulations are designed as follows: <br />
•	All vehicles are equipped with 5G technology, where SUMO is used to generate mobility.<br />
•	There are two distinct groups of vehicles: senders and receivers.<br />
•	Message exchange between vehicles is made via the multicast address (i.e., 225.0.0.0).<br /><br />
As previously stated, vehicles are separated into two groups (i.e., senders and receivers) and we generated four maps: <br />
•	the first map has a total of 45 vehicles, where 10 are senders (from this total, two vehicles are attackers) and 35 receivers; <br />
•	the second map also has 45 vehicles, where 10 are senders (from this total, four vehicles are attackers) and 35 receivers; <br />
•	the third map has a total of 70 vehicles, where 15 are senders (from this total, seven are attackers) and 55 receivers; <br />
•	finally, the fourth map has 100 vehicles, where 19 are senders (from this total, nine vehicles are attackers) and 81 receivers. <br />
In addition, each simulation lasts a total of 230 s. However, to enable more mobility/movement of the vehicles, they exchange packets at second 170.<br />

Additionally, all datasets have the following features:<br />
•	timeSec — this feature indicates the simulation time at which a packet is sent or received. In our dataset, we are considering only metrics of received packets; <br />
•	txRx — a tag to indicate whether a packet was sent (tx) or received (rx);<br />
•	nodeId — refers to the receiver node ID; <br />
•	imsi — is the International Mobile Subscriber Identity, which is an identifier assigned with the SIM (Subscriber Identity Module) card; <br />
•	srcIp — the IP address of a sender node; <br />
•	dstIp — the IP address of a receiver node; <br />
•	packetSizeBytes — it refers to the packet size in bytes. Each sender node uses a different size to increase randomness; <br />
•	srcPort — refers to the port where the sender nodes are sending the packets; <br />
•	dstPort — refers to the port where the receiver nodes are receiving the packets; <br />
•	pktSeqNum — refers to the sequence of transmitted packets; <br />
•	delay — the difference between the reception time of a packet and its sending time; <br />
•	jitter — it uses the RFC 1889 format; <br />
•	coord_x — is the “x” coordinate on the map generated in SUMO; <br />
•	coord_y — is the “y” coordinate on the map generated in SUMO; <br />
•	speed — is the speed of the vehicle in meters per second; <br />
•	isAttack — is the class of benign (class 0) packet or malign (class 1) packet.<br />

# Cite our work
Sousa B, Magaia N, Silva S. An Intelligent Intrusion Detection System for 5G-Enabled Internet of Vehicles. Electronics. 2023; 12(8):1757. https://doi.org/10.3390/electronics12081757
