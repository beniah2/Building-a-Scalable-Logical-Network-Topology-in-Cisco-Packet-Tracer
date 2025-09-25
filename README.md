### Building a Scalable Logical Network Topology in Cisco Packet-Tracer

# Story Part 1: The Assignment

It was a rainy Monday morning when I received a call from TechNova Solutions, a fast-growing remote company struggling with their internal network. Their employees were spread across three departments—Finance, Research, and Customer Support—but their network was flat, unreliable, and unable to handle the growing demand. The CTO tasked me with designing a scalable logical network topology that would not only connect all departments securely but also make future expansions easier.
The requirements:

3 Routers (for inter-departmental communication)

3 Switches (one per department)

12 End Devices (4 per department)

My mission: Design, configure, and demonstrate the new network topology using Cisco Packet Tracer.

---

## Action 1: Setting Up the Base Network

First, I laid out the physical devices on the Packet Tracer workspace.

## Command

Drag 3 Routers onto the workspace.

Drag 3 Switches (2960 model) onto the workspace.

Add 12 end devices (PCs or Laptops). Place 4 devices per switch.

<img width="1593" height="612" alt="image" src="https://github.com/user-attachments/assets/56188050-9865-45c7-bfbc-83f927771fcd" />

---

# Story Part 2: Connecting the Departments

Each department needed to be structured in a way that made sense. Finance wanted to be isolated but still able to send reports to Research and Customer Support. Research needed high bandwidth for data transfers. Customer Support required stable VoIP and client communication.

So, I grouped devices as follows:

Finance Dept → Switch 1 → Router 1

Research Dept → Switch 2 → Router 2

Support Dept → Switch 3 → Router 3

Each router would be interconnected for cross-departmental communication.

---

Action 2: Cabling the Network

I then connected all devices logically using appropriate cables.

## Command

Use Copper Straight-Through cables to connect PCs → Switches.

Use Copper Straight-Through cables to connect Switches → Routers.

Use Serial Connections between Routers.

<img width="1391" height="639" alt="image" src="https://github.com/user-attachments/assets/bebc78a7-a4f2-47e9-a21f-c1ff4a80b384" />

---

## Story Part 3: IP Addressing Scheme

To avoid confusion, I designed a clear IP addressing plan:

Finance Network: 192.168.1.0/24

Research Network: 192.168.2.0/24

Support Network: 192.168.3.0/24

Routers would act as gateways for each department.

## Action 3: Assigning IP Addresses

# Command

On each PC: Desktop → IP Configuration → Assign IP + Subnet + Gateway

Example (Finance PC1):

IP: 192.168.1.2

Subnet: 255.255.255.0

Gateway: 192.168.1.1

Repeat for all devices in all the departments.

<img width="1052" height="820" alt="image" src="https://github.com/user-attachments/assets/b4bb5e01-88fc-4f5c-bd93-7c03d0682bc2" />




