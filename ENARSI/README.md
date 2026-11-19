# ENARSI Labs
### CCNP ENARSI (300-410) troubleshooting labs in GNS3, each built around one fault

Part of the [GNS3 labs repository](../README.md).

---

## Summary

My ENARSI labs, built and tested in GNS3 on Cisco IOSv. Each lab has the topology and addressing plan, and a "Break-It" exercise: a fault injected on purpose, the symptom it caused, and how I found and fixed it with show commands.

## Lab Environment

| Component | Specification | Purpose |
| :--- | :--- | :--- |
| **Network Emulator** | GNS3 Server / Client v3.1 | Topology |
| **Router** | Cisco IOSv 15.9(3)M12 (QEMU), 1 vCPU / 512 MB | BGP, routing, AAA client |
| **AAA Server** | FreeRADIUS 3 (Docker, host network) | RADIUS for SSH logins |

IOSv images are not included in this repo.

---

## Labs

### Module 1: BGP Fundamentals

| Lab | Title | Key Technologies | Documentation |
| :---: | :--- | :--- | :---: |
| **1.1** | BGP Tables and Administrative Distance | eBGP, BGP table vs RIB, AD, `rib-failure`, `source lo0` | [View Lab](Module%201%20%E2%80%93%20BGP%20Fundamentals/Lab%201%20%E2%80%93%20BGP%20Tables%20and%20AD/README.md) |

### Module 2: AAA

| Lab | Title | Key Technologies | Documentation |
| :---: | :--- | :--- | :---: |
| **2.1** | RADIUS Login Fails | AAA, RADIUS auth-port 1812 vs 1645, `test aaa`, local fallback | [View Lab](Module%202%20%E2%80%93%20AAA/Lab%201%20%E2%80%93%20RADIUS%20Login%20Fails/README.md) |
