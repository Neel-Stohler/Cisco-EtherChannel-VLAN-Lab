# Cisco EtherChannel and VLAN Lab

A Cisco Packet Tracer lab demonstrating VLAN segmentation, EtherChannel configuration, and network redundancy.

## Network Topology

![Network Topology](screenshots/topology.png)

**Components:**
- 1 router
- 2 switches
- 4 PCs
- 2 VLANs
- 1 EtherChannel with 3 physical links

## Implemented Features

- VLAN creation and access port configuration
- EtherChannel configuration
- IP address planning
- Network connectivity testing using ICMP ping
- Link redundancy and failover testing
- Network documentation and interface labeling

## EtherChannel Verification

The EtherChannel configuration was verified using `show etherchannel summary`. The physical interfaces were checked to ensure they were successfully bundled into the logical Port-Channel.

![EtherChannel Summary](screenshots/etherchannel-summary.png)

## Connectivity and Failover Testing

Connectivity was tested using ICMP ping. To verify redundancy, one physical EtherChannel interface (`Fa0/1`) was disabled using `shutdown`.

Communication between the PCs remained functional through the remaining active links. The interface was subsequently restored using `no shutdown`.

![EtherChannel Failover](screenshots/etherchannel-failover.png)

![Ping Test](screenshots/ping-test.png)

## Tools

- Cisco Packet Tracer
- Cisco IOS CLI


Screenshots:
<img width="1920" height="1080" alt="Screenshot from 2026-10-11 21-11-26" src="https://github.com/user-attachments/assets/ff210ac9-bf32-407e-aff2-bfeda25335f3" />
<img width="1920" height="1080" alt="Screenshot from 2026-10-11 21-09-54" src="https://github.com/user-attachments/assets/a77959c0-3cb4-4f58-a92f-32a2d57c3137" />


