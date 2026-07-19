# Multi-Branch Corporate Network with OSPF, DHCP, and ACL

This repository contains an enterprise-grade multi-branch network topology simulated using **Cisco Packet Tracer**. The project demonstrates advanced network infrastructure design, dynamic routing, automated IP addressing, and robust network security policies.

## 🛠️ Technologies & Protocols Implemented
* **Simulation Tool:** Cisco Packet Tracer
* **Core Concepts:** OSPF (Open Shortest Path First), DHCP (Dynamic Host Configuration Protocol), ACL (Access Control Lists), VLANs, Subnetting.

## 🏗️ Architecture & Configuration Overview
The network infrastructure simulates a Headquarters (HQ) and a Branch Office connected via a WAN link, featuring:

1. **Dynamic Routing (OSPF):** 
   Configured OSPF Area 0 across HQ and Branch routers to establish dynamic, seamless communication between different subnets without manual static routes.
2. **Automated IP Management (DHCP):** 
   Configured router-based DHCP pools to automatically assign IP addresses, subnet masks, and default gateways to end devices in both the HQ (HR & IT departments) and the Branch office.
3. **Enterprise Security (Extended ACL):** 
   Implemented rigorous security policies using Extended Access Control Lists. 
   * **Rule 1:** The HR Department is strictly denied access to the Branch network.
   * **Rule 2:** The IT Department retains full communication privileges with the Branch network.

## 🚀 How to Test the Project
1. Download the `Multi_Branch_Network_OSPF_ACL.pkt` file.
2. Open it using Cisco Packet Tracer.
3. **Test DHCP:** Check the IP configuration of any PC to verify successful DHCP allocation.
4. **Test OSPF & ACL Security:** 
   * Open the Command Prompt on an **HR PC** and ping a Branch PC (Expected result: `Destination host unreachable` due to ACL blocking).
   * Open the Command Prompt on an **IT PC** and ping a Branch PC (Expected result: Successful ICMP echo replies, proving OSPF routing is active and allowed by ACL).

## 👤 Author
**Heshani Nethmini**
