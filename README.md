# DHCP Relay Configuration
What if some clients are not directly connected to the DHCP server? Almost similar to the [previous simulation](https://github.com/eightball270/Basic-VLAN-and-DHCP-Server?tab=readme-ov-file#basic-vlan-and-dhcp-server), but in this simulation using 2 routers in order to configure **DHCP relay**. So some clients still get automatic IP configuration even though they are not directly connected to the DHCP server.

## Technology Used
1. Cisco Packet Tracer
2. GNS3 (MikroTik)

## Requirements
1. 2 Routers and a Switch
2. Client PCs
3. Access Point and Client Wireless devices*

*) optional if creating a WLAN connection, but can be replaced with a regular LAN (Client PCs)

## Configuration Completed
1. Divide into 4 vlans on the router and switch
2. Assign an IP address to each router as a gateway
3. Inter-router connection
4. DHCP server on first router (R1)
5. Static routing on router R1 to the network addresses of some clients
6. DHCP relay on second router (R2) that is directly connected to some clients
7. SSID and password on a Access Point (for WLAN connection)

## DHCP Relay
### Cisco

![DHCP Relay.png](https://github.com/eightball270/DHCP-Relay-Configuration/blob/main/Cisco/DHCP%20Relay.png)

[Project File Link](https://github.com/eightball270/DHCP-Relay-Configuration/blob/main/Cisco/DHCP%20Relay.pkt)

The DHCP results of the representative VLAN are as follows:

![DHCP Relay (1).png](https://github.com/eightball270/DHCP-Relay-Configuration/blob/main/Cisco/DHCP%20Relay%20(1).png) ![DHCP Relay (2).png](https://github.com/eightball270/DHCP-Relay-Configuration/blob/main/Cisco/DHCP%20Relay%20(2).png) ![DHCP Relay (3).png](https://github.com/eightball270/DHCP-Relay-Configuration/blob/main/Cisco/DHCP%20Relay%20(3).png) ![DHCP Relay (4).png](https://github.com/eightball270/DHCP-Relay-Configuration/blob/main/Cisco/DHCP%20Relay%20(4).png)

## MikroTik

![DHCP Relay (MikroTik).png](https://github.com/eightball270/DHCP-Relay-Configuration/blob/main/MikroTik/DHCP%20Relay%20(MikroTik).png)

[Project File Link](https://github.com/eightball270/DHCP-Relay-Configuration/blob/main/MikroTik/DHCP%20Relay.gns3project.7z)

The DHCP results of the representative VLAN are as follows:

![DHCP Relay (MikroTik) (1).png](https://github.com/eightball270/DHCP-Relay-Configuration/blob/main/MikroTik/DHCP%20Relay%20(MikroTik)%20(1).png) ![DHCP Relay (MikroTik) (2).png](https://github.com/eightball270/DHCP-Relay-Configuration/blob/main/MikroTik/DHCP%20Relay%20(MikroTik)%20(2).png) ![DHCP Relay (MikroTik) (3).png](https://github.com/eightball270/DHCP-Relay-Configuration/blob/main/MikroTik/DHCP%20Relay%20(MikroTik)%20(3).png) ![DHCP Relay (MikroTik) (4).png](https://github.com/eightball270/DHCP-Relay-Configuration/blob/main/MikroTik/DHCP%20Relay%20(MikroTik)%20(4).png)
