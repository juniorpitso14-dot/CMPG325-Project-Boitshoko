# CMPG325-Project-Boitshoko
Individual Semester Project for Boitshoko Health Research Unit - NetAcad Portfolio.

 # CMPG 325 - Computer Networks Semester Project
### Academic Portfolio: Boitshoko Health Research Unit (Klerksdorp)

## Student Information
* **Name:** PITSO, J
* **Student Number:** 39046338
* **Project ID:** CMPG325-2026-111
* **Client ID:** CLI-111

---

## Milestone 1: Client Design Review Submission

### 1. Project Structural Organization
This repository serves as the official technical documentation repository and file proof of evidence ledger for the design, deployment validation, and optimization testing of the Boitshoko Health network implementation.

### 2. Core Topology Strategy
The physical footprint isolates internal assets into separate subnet branches directly at the Layer 3 edge boundaries on the central gateway router. 
* **Department A (Research):** Configured on a `/26` partition ensuring baseline containment for active workstations and 8 added positions brought on by Change Request 1.
* **Department B (Administration):** Configured on a `/27` perimeter partition.
* **Future Department Space:** Blocked via an unassigned `/27` range to allow seamless expansion next year.

### 3. Verification Directory Reference Maps
* View baseline project design files here: `/documentation/`
* Track structural simulation progression designs here: `/topology/`
* Source baseline network builds here: `/packet-tracer/`

---
*Confidential Student Academic Submission - NWU Faculty of Engineering, Computer Science and Information Systems.*
