# 🏢 Main Office & Branch Office Network Design & Configuration

### **Computer Networks – Semester Project**

This project presents a complete enterprise-level network design connecting a **Main Office** and a **Branch Office**.
It includes VLAN segmentation, OSPF routing, DHCP configuration, WAN connectivity, and full documentation for academic and practical evaluation.

---

## 📌 **Project Overview**

This network infrastructure is built to support secure, scalable, and efficient communication between two offices using Cisco networking devices.

The project covers:

* VLAN-based segmentation for multiple departments
* Inter-VLAN routing using router-on-a-stick
* Dynamic routing using **OSPF**
* DHCP automation for every VLAN
* WAN serial link between Main & Branch offices
* Full connectivity testing (ping, traceroute, routing tables)

The design follows enterprise networking standards, ensuring optimized routing, separation of broadcast domains, and controlled departmental communication.

---

## 🎯 **Objectives**

### **Primary Objectives**

* Build a complete network covering Main & Branch Offices
* Implement VLANs for separate departments
* Configure OSPF dynamic routing
* Provide secure WAN communication
* Automate addressing using DHCP
* Ensure end-to-end connectivity between all PCs and offices
* Produce professional documentation and diagrams

### **Secondary Objectives**

* Implement basic network security (ACLs, Port Security, DHCP snooping)
* Use correct subnetting, gateway allocation, and structured IP planning
* Create scalable design for future growth

---

## 📌 **Scope of Work**

* Complete network design for both offices
* VLAN creation & access-port assignments
* Inter-VLAN routing via sub-interfaces
* OSPF routing configuration
* DHCP pools for each department
* WAN setup using serial interfaces
* Routing table verification & connectivity testing
* Creation of professional topology diagrams
* Final project documentation

---

## 🔧 **Tools & Technologies Used**

| Tool / Device              | Purpose                    |
| -------------------------- | -------------------------- |
| Cisco Packet Tracer        | Simulation & configuration |
| Cisco Routers (ISR)        | Routing, OSPF, WAN         |
| Cisco Switches (2960/3560) | VLANs, trunking            |
| Windows/Generic Servers    | DHCP, DNS, Web             |
| PCs & Laptops              | End-user devices           |
| draw.io / Lucidchart       | Diagramming                |

---

## 🗺️ **Network Topology**

### **Main Office Contains**

* 2 Switches
* 1 Router
* 4 VLAN Departments: HR, IT, Finance, Admin
* Server Room (DHCP, DNS, Web)

### **Branch Office Contains**

* 1 Router
* 1 Switch
* 3 VLAN Departments
* User PCs

Both routers communicate using a **Serial WAN Link**, and all inter-office traffic is routed using **OSPF**.

---

## 🏷️ **VLAN Design**

| VLAN ID | Department       | Location      |
| ------- | ---------------- | ------------- |
| 10      | HR               | Main Office   |
| 20      | IT               | Main Office   |
| 30      | Finance          | Main Office   |
| 40      | Admin/Management | Main Office   |
| 50      | Branch Users     | Branch Office |

Each VLAN has its own IP subnet.

---

## 💻 **Main Office (R1) – Key Configurations**

* DHCP pools for all VLANs
* Router-on-a-stick sub-interfaces
* OSPF area 0 routing
* WAN setup on Serial 0/1/0

✔ All VLANs receive IP addresses
✔ Inter-VLAN routing working
✔ OSPF adjacency formed

(Full configuration included in documentation.)

---

## 🖧 **Branch Office (R2) – Key Configurations**

* Local DHCP services
* VLANs for three departments
* OSPF routing configuration
* Serial link to Main Office

✔ Branch → Main communication successful
✔ Routes learned dynamically using OSPF

(Full configuration included in documentation.)

---

## 🧪 **Testing & Verification**

Commands used:

* `show ip interface brief`
* `show ip route`
* `show dhcp lease`
* `ping` tests across VLANs & offices
* `traceroute` for path verification

**All tests successful**, including:
✔ DHCP assignments
✔ Inter-VLAN communication
✔ Inter-office connectivity
✔ OSPF adjacency
✔ Default routing behavior

---

## 🏁 **Conclusion**

This project successfully demonstrates a fully functional, secure, and scalable enterprise network.
It covers VLAN segmentation, routing, DHCP, WAN connectivity, documentation, and real-world network design principles suitable for professional environments.

---

## 📂 **Repository Structure**

```
📁 CN-Project-Banking-Network
│── 📄 README.md
│── 📄 Zaeem Bilal (62630) CN Project Documentation.pdf
│── 💾 PacketTracer File
```

---

## 🔗 **Project Repository**

You can find the entire project at:
👉 **[https://github.com/Zaeem-Alpha/CN-Project-3rd-Sem]**

