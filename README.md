# Home Network Simulation

This project simulates a small home/office network using Cisco Packet Tracer. 
It demonstrates wired connections between PCs and switches, router configuration, DHCP setup, and end-to-end connectivity testing.

## Topology Overview
- 4 PCs connected via 2 switches to 1 router
- PCs divided into 2 subnets:
  - Subnet 1: AYAZPC, BOBPC → Switch1 → Router
  - Subnet 2: DAVEPC, JOHNPC → Switch2 → Router
- Router interfaces configured for inter-subnet communication

## Features
- Wired connections from PCs to switches and router
- Router configured with multiple interfaces
- Static IP and default gateway configuration
- DHCP for dynamic IP assignment (if enabled)
- Ping tests to verify connectivity across all devices

## IP Configuration
| Device  | IP Address    | Subnet Mask     | Default Gateway |
|---------|---------------|----------------|----------------|
| AYAZPC  | 192.168.1.10   | 255.255.255.0  | 192.168.1.1    |
| BOBPC     | 192.168.1.11   | 255.255.255.0  | 192.168.1.1    |
| DAVEPC     | 192.168.2.10   | 255.255.255.0  | 192.168.2.1    |
| JOHNPC     | 192.168.2.11   | 255.255.255.0  | 192.168.2.1    |
| Router  | 192.168.1.1 / 192.168.2.1 | 255.255.255.0 | - |

## Screenshots
- Topology view: ![Topology](https://github.com/ayazcoskun/home-network-simulation/blob/39320c4a8297e3c001cd84f8825d1b608c3c0772/topology.png.png)
- Router configuration: ![Router Config](router_config.png)
- Ping tests from AYAZPC to DAVEPC: ![Ping Test](ping_test.png)

## How to Test
1. Open the `.pkt` file in Cisco Packet Tracer.
2. Verify IP addresses for all devices.
3. Test connectivity using ping commands between PCs across different subnets.
4. Optionally, turn off/on devices via Physical tab to simulate power outages.

## What I Learned
- How to create a multi-subnet network using switches and routers
- Basic routing and IP addressing
- Configuring default gateways for inter-subnet communication
- Using ping tests to troubleshoot network connectivity
