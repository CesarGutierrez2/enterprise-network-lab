# enterprise-network-lab

PROJECT OVERVIEW
A multi-site enterprise network simulation built in Cisco Packet Tracer 9.0 demonstrating real-world networking skills including VLAN segmentation, inter-VLAN routing, centralized DHCP, and ACL-based security controls 

SKILLS DEMONSTRATED
- VLAN segmentation and trunk configuration
- Router-on-a-stick inter-VLAN routing
- Centralized DHCP with ip helper-address relay
- ACL-based security controls
- Static routing over WAN link
- Network troubleshooting and verification

NETWORK TOPOLOGY
- HQ site: 5 VLANS (HR, IT, Finance, Guest, Management)
- Branch site: Remote office connected via WAN link
- WAN: Point-to-point 10.0.0.0/30 link

IP ADDRESSING SCHEME 
VLAN  NAME     NETWORK         GATEWAY
10    HR    192.168.10.0/24  192.168.10.1
20    IT    192.168.20.0/24  192.168.20.1
30  Finance 192.168.30.0/24  192.168.30.1
40  Guest   192.168.40.0/24  192.168.40.1
50  Branch  192.168.50.0/24  192.168.50.1

SECURITY CONTROLS
- HR and Finance VLANs are mutually isolated via ACL
- Guest VLAN is isolated from all internal networks
- IT VLAN has full administrative access

TROUBLESHOOTING NOTES
- Resolved DHCP failure caused by SERVER1 port not assigned to VLAN 20
- Identified and corrected default gateway misconfiguration on IT-PC1 caused by DHCP cycling in Packet Tracer
- Investigated branch ACL routing asymmetry and documented as known limitation of Packet Tracer static routing simulation

TOOLS USED
- Cisco Packet Tracer 9.0
- Cisco IOS CLI
