# Star Wars Network Lab

## Project Overview
A simple networking lab created in Cisco Packet Tracer inspired by the Star Wars universe.  
The goal: connect the Rebel base on **Yavin 4** with the Jedi training grounds on **Dagobah** through the **R2-D2 router**.

---

## Topology
- Router: **R2-D2 (Cisco 1941)**
- Switches: **SW-Yavin4**, **SW-Dagobah**
- PCs: **Luke-PC**, **Yoda-PC**

---

## IP Addressing
| Device | Interface | IP | Mask | Gateway |
|---------|------------|----|--------|----------|
| R2-D2 | G0/1 | 192.168.1.1 | 255.255.255.0 | - |
| SW-Yavin4 | VLAN1 | 192.168.1.2 | 255.255.255.0 | 192.168.1.1 |
| SW-Dagobah | VLAN1 | 192.168.1.3 | 255.255.255.0 | 192.168.1.1 |
| Luke-PC | Fa0 | 192.168.1.10 | 255.255.255.0 | 192.168.1.1 |
| Yoda-PC | Fa0 | 192.168.1.20 | 255.255.255.0 | 192.168.1.1 |

---

## Configuration Files
All CLI configurations are available in the `config/` directory.

---

## Testing
- Ping between Luke-PC and Yoda-PC  
- Ping between router and switches  
- (Optional) SSH access to R2-D2

---

## Technologies Used
- Cisco Packet Tracer 8.x  
- VLAN Management  
- IP Routing  
- Banner MOTD  
- SSH (optional)

---

## Author
**Piotr Brzeziński**  
Educational networking project created as part of CCNA learning.
