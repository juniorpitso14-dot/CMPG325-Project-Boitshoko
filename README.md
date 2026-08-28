# CMPG325 Computer Networks Project

## Botshoko Health Research Unit – Klerksdorp

### Student Information

**Student:** Junia Pitso  
**Student Number:** 39064338  
**Module:** CMPG325 – Computer Networks  
**Project:** Individual Semester Project  
**Client:** Botshoko Health Research Unit  
**Industry:** Research  
**Location:** Klerksdorp  

---

## 1. Project Overview

This project involves the design, implementation, configuration and testing of a computer network for the Botshoko Health Research Unit in Klerksdorp.

The network was designed and simulated using Cisco Packet Tracer. The assigned addressing block for the project is 192.168.50.0/24.

The network provides connectivity between the different departments of the organisation while using VLANs to logically separate departmental traffic.

The project also implements Port Security as the assigned networking challenge.

---

## 2. Client Requirements

The network must:

- Provide connectivity between the required departments.
- Provide an appropriate network topology and device arrangement.
- Use the assigned 192.168.50.0/24 addressing block.
- Configure routers, switches and end devices.
- Provide successful end-to-end connectivity.
- Implement Port Security.
- Accommodate eight additional staff members in one department without redesigning the network.
- Provide evidence of configuration and testing.
- Document troubleshooting and design decisions.

---

## 3. Network Design

The proposed network consists of:

- 1 router
- 2 switches
- Research Department
- Administration Department
- Human Resources Department
- IT Department

VLANs are used to logically separate the departments.

| VLAN | Department |
|---|---|
| 10 | Research |
| 20 | Administration |
| 30 | Human Resources |
| 40 | IT |
| 99 | Management |

---

## 4. IP Addressing

The assigned network block is:

192.168.50.0/24

VLSM was used to divide the address block into suitable subnets.

| VLAN | Network | Mask | Gateway |
|---|---|---|---|
| 10 | 192.168.50.0/26 | 255.255.255.192 | 192.168.50.1 |
| 20 | 192.168.50.64/27 | 255.255.255.224 | 192.168.50.65 |
| 30 | 192.168.50.96/28 | 255.255.255.240 | 192.168.50.97 |
| 40 | 192.168.50.112/28 | 255.255.255.240 | 192.168.50.113 |
| 99 | 192.168.50.128/28 | 255.255.255.240 | 192.168.50.129 |

---

## 5. Networking Challenge

### Port Security

Port Security was implemented on switch access ports to restrict the devices that are permitted to connect to protected switch ports.

Sticky MAC address learning was used and the maximum number of permitted MAC addresses was configured as one.

The violation mode was configured as shutdown.

---

## 6. Client Change Request

The client requested eight additional staff members in one department.

The Research Department was selected for the expansion.

The original design allocated sufficient address capacity and reserved switch ports for additional Research computers.

Therefore, the eight additional staff members can be added without redesigning the network.

---

## 7. Testing

Testing includes:

- Same-VLAN connectivity
- Inter-VLAN connectivity
- Router gateway connectivity
- Connectivity between switches
- Connectivity of newly added staff
- Port Security verification
- Port Security violation testing

---

## 8. Evidence

Screenshots and configuration evidence are included in the Evidence directory.

---

## 9. Packet Tracer File

The completed Cisco Packet Tracer implementation is available in:

`04_Packet_Tracer/Botshoko_Health_Research_Network.pkt`

---

## 10. Conclusion

The completed network provides a structured and scalable network solution for the Botshoko Health Research Unit.

The design provides departmental segmentation through VLANs, routing between VLANs, appropriate IP addressing, Port Security and capacity for the requested additional staff.
