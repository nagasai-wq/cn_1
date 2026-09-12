# Lab 1.1: Study of Network Devices in Detail and Connect Computers in Local Area Network (LAN)

## Aim
To study network devices in detail and connect computers in a Local Area Network (LAN) using a switch, Ethernet cables, and IP configuration.

---

## 1. Study of Network Devices

* **Network Interface Card (NIC):** A hardware component that connects a computer to a network, assigning a unique physical (MAC) address to the device.
* **Hub:** A physical-layer device that broadcasts incoming data frames to all connected ports (obsolete due to high collisions).
* **Switch:** An intelligent data link layer device that forwards data packets to specific ports based on MAC addresses.
* **Router:** A network layer device that routes data packets between different networks using IP addresses.
* **Bridge:** A device that connects two separate network segments and filters traffic based on MAC addresses.
* **Repeater:** A device that receives and regenerates signals to extend the transmission distance across a network.
* **Gateway:** A node that acts as a translator between two networks using different protocols.

---

## 2. LAN Setup & IP Configuration

### Network Topology
* **Topology:** Star Topology
* **Hardware Used:** 3 PCs, 1 Unmanaged Ethernet Switch, Cat5e/Cat6 RJ45 Ethernet Cables

### IP Assignment Table

| Computer Name | IP Address | Subnet Mask | Default Gateway |
| :--- | :--- | :--- | :--- |
| **PC1** | `192.168.1.10` | `255.255.255.0` | `192.168.1.1` |
| **PC2** | `192.168.1.11` | `255.255.255.0` | `192.168.1.1` |
| **PC3** | `192.168.1.12` | `255.255.255.0` | `192.168.1.1` |

---

## 3. Procedure

1. **Physical Connectivity:** Connected PC1, PC2, and PC3 to the Ethernet switch using Cat5e/Cat6 RJ45 cables. Verified physical connection via switch link LED indicators.
2. **IP Configuration:** Assigned static IPv4 addresses, subnet masks, and default gateways on each host using standard OS network settings.
3. **Verification:** Executed `ipconfig` (Windows) / `ifconfig` (Linux) to verify adapter configurations.
4. **Connectivity Testing:** Ran `ping` commands from PC1 to verify reachable communication across all hosts on the local subnet.

---

## 4. Execution & Verification Output

### Verifying Local Configuration (PC1)
```cmd
C:\Users\PC1> ipconfig

Ethernet adapter Ethernet0:
   Connection-specific DNS Suffix  . :
   IPv4 Address. . . . . . . . . . . : 192.168.1.10
   Subnet Mask . . . . . . . . . . . : 255.255.255.0
   Default Gateway . . . . . . . . . : 192.168.1.1
