# Telnet Configuration Lab

This project demonstrates how to configure remote access to a Cisco router using **Telnet** with local authentication.

---

## Project Objective

- Configure basic router settings
- Create local user authentication
- Enable remote access using Telnet
- Restrict VTY lines to Telnet only

---

## Topology

![Topology](docs/topology.png)

### Network Details

- Network: 192.168.1.0/24
- Router: Cisco 2911
- Switch: Cisco 2960
- PCs:
  - PC0 → 192.168.1.2
  - PC1 → 192.168.1.3
  - PC2 → 192.168.1.4

---

## What is Telnet?

Telnet is a remote access protocol that allows administrators to access and manage network devices over TCP port 23.

Telnet sends credentials in plain text, which makes it insecure for production environments. It is mainly used for lab and learning purposes.

---

## What is VTY?

VTY (Virtual Terminal Lines) are logical ports on Cisco devices that allow remote connections (Telnet or SSH).

Example:
```
line vty 0 15
```
This allows up to 16 remote sessions.

---

## Configuration Summary

- Hostname configured
- Enable password set
- Local username created
- VTY lines configured for Telnet
- Local database authentication enabled

---

## Project Files

- `docs/` → Contains topology image
- `packet-tracer/` → Packet Tracer file
- `configs/` → Router configuration files

---

## How to Test

From any PC:

```
telnet 192.168.1.1
```

Enter username: `Admin`  
Enter password: `cisco`

---

## Author

Ankit Kuttarmare  
