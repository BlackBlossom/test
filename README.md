Excellent strategy. If you can answer these **25 questions confidently with explanations**, you'll handle most CN practical vivas.

---

# 1. What is the OSI Model?

### Answer

OSI stands for **Open Systems Interconnection Model**.

It is a **7-layer reference model** developed by ISO to standardize communication between computer systems.

The OSI model explains how data travels from one computer to another through different layers.

### Layers

1. Physical Layer
2. Data Link Layer
3. Network Layer
4. Transport Layer
5. Session Layer
6. Presentation Layer
7. Application Layer

### Example

When you open Google:

* Application Layer creates request
* Transport Layer adds TCP
* Network Layer adds IP
* Data Link Layer adds MAC
* Physical Layer sends bits

### Viva Follow-up

**Why OSI Model?**

To divide networking into manageable layers and simplify troubleshooting.

---

# 2. How Many Layers are in OSI?

### Answer

OSI has **7 layers**.

Mnemonic:

**Please Do Not Throw Sausage Pizza Away**

| Layer | Name         |
| ----- | ------------ |
| 7     | Application  |
| 6     | Presentation |
| 5     | Session      |
| 4     | Transport    |
| 3     | Network      |
| 2     | Data Link    |
| 1     | Physical     |

---

# 3. Difference Between Hub and Switch

| Hub             | Switch                    |
| --------------- | ------------------------- |
| Layer 1         | Layer 2                   |
| Uses no address | Uses MAC address          |
| Broadcasts data | Sends to destination only |
| Slow            | Fast                      |
| More collisions | Fewer collisions          |

### Viva Answer

A hub sends data to all devices, while a switch forwards data only to the intended destination using MAC addresses.

---

# 4. Difference Between Switch and Router

| Switch                       | Router                      |
| ---------------------------- | --------------------------- |
| Layer 2                      | Layer 3                     |
| Uses MAC Address             | Uses IP Address             |
| Connects devices in same LAN | Connects different networks |

### Example

Switch:

```text
PC1 ↔ PC2
```

Router:

```text
Home Network ↔ Internet
```

---

# 5. What is a MAC Address?

### Answer

MAC (Media Access Control) Address is the physical address of a network interface card.

### Example

```text
00:1A:2B:3C:4D:5E
```

### Length

```text
48 bits
```

### Purpose

Used for communication inside a LAN.

### Layer

Data Link Layer

---

# 6. What is an IP Address?

### Answer

IP Address is a logical address assigned to a device for communication across networks.

### Example

```text
192.168.1.10
```

### Purpose

Identifies devices globally or within networks.

### Layer

Network Layer

---

# 7. Difference Between MAC and IP

| MAC              | IP                    |
| ---------------- | --------------------- |
| Physical address | Logical address       |
| Layer 2          | Layer 3               |
| Fixed (usually)  | Can change            |
| Used in LAN      | Used between networks |

### Viva Line

MAC identifies the device locally, while IP identifies the device logically across networks.

---

# 8. What is ARP?

### Answer

ARP stands for **Address Resolution Protocol**.

It converts:

```text
IP Address → MAC Address
```

### Example

PC wants to send data to:

```text
192.168.1.20
```

It first asks:

> Who has 192.168.1.20?

The destination replies with its MAC address.

---

# 9. What is DHCP?

### Answer

DHCP stands for **Dynamic Host Configuration Protocol**.

It automatically assigns:

* IP Address
* Subnet Mask
* Gateway
* DNS

### DHCP Process

**DORA**

* Discover
* Offer
* Request
* Acknowledge

### Ports

Server = 67

Client = 68

---

# 10. What is DNS?

### Answer

DNS stands for **Domain Name System**.

It converts:

```text
google.com
```

into

```text
142.x.x.x
```

### Why Needed?

Humans remember names more easily than IP addresses.

### Port

53

---

# 11. What is NAT?

### Answer

NAT stands for **Network Address Translation**.

It converts:

```text
Private IP → Public IP
```

### Example

Home devices:

```text
192.168.1.x
```

share one public IP through NAT.

### Advantage

Conserves IPv4 addresses.

---

# 12. What is Ping?

### Answer

Ping is a utility used to test connectivity between two devices.

### Command

```bash
ping google.com
```

### Uses

* Check connectivity
* Measure delay
* Troubleshoot networks

---

# 13. What is ICMP?

### Answer

ICMP stands for **Internet Control Message Protocol**.

Used for:

* Error reporting
* Diagnostics
* Ping

### Examples

* Echo Request
* Echo Reply
* Destination Unreachable

### Layer

Network Layer

---

# 14. What is TCP?

### Answer

TCP stands for **Transmission Control Protocol**.

It provides:

* Reliable communication
* Error recovery
* Sequencing
* Acknowledgements

### Examples

Used by:

* HTTP
* HTTPS
* FTP

---

# 15. What is UDP?

### Answer

UDP stands for **User Datagram Protocol**.

It provides:

* Fast communication
* No connection setup
* No acknowledgements

### Examples

Used in:

* Gaming
* Video Streaming
* DNS

---

# 16. Difference Between TCP and UDP

| TCP                 | UDP            |
| ------------------- | -------------- |
| Reliable            | Unreliable     |
| Connection-oriented | Connectionless |
| Uses ACK            | No ACK         |
| Slower              | Faster         |

### Viva Answer

TCP prioritizes reliability while UDP prioritizes speed.

---

# 17. What is CRC?

### Answer

CRC stands for **Cyclic Redundancy Check**.

It is an error detection technique.

### Working

1. Sender performs modulo-2 division.
2. Remainder attached to data.
3. Receiver performs same division.
4. Non-zero remainder means error.

### Layer

Data Link Layer

---

# 18. What is Framing?

### Answer

Framing is the process of dividing a stream of bits into smaller units called frames.

### Layer

Data Link Layer

### Why Needed?

Receiver must identify:

* Frame start
* Frame end

---

# 19. What is Bit Stuffing?

### Answer

Bit Stuffing inserts a:

```text
0
```

after every sequence of:

```text
11111
```

### Purpose

Prevent accidental appearance of frame flag.

### Used In

HDLC Protocol

---

# 20. What is Dijkstra Algorithm?

### Answer

Dijkstra is a shortest-path routing algorithm.

It finds the minimum-cost path from source to destination.

### Used By

OSPF

### Layer

Network Layer

---

# 21. What is OSPF?

### Answer

OSPF stands for:

**Open Shortest Path First**

### Type

Link State Routing Protocol

### Uses

Dijkstra Algorithm

### Metric

Cost

### Advantage

Fast convergence and efficient routing.

---

# 22. What is RIP?

### Answer

RIP stands for:

**Routing Information Protocol**

### Type

Distance Vector Routing Protocol

### Metric

Hop Count

### Maximum Hops

```text
15
```

### Limitation

Not suitable for large networks.

---

# 23. What is VLAN?

### Answer

VLAN stands for:

**Virtual Local Area Network**

It logically divides a switch into multiple separate networks.

### Example

```text
VLAN 10 → HR
VLAN 20 → Sales
```

### Advantages

* Better security
* Reduced broadcasts
* Easier management

---

# 24. What is Packet Tracer?

### Answer

Cisco Packet Tracer is a network simulation software developed by Cisco.

### Uses

* Design networks
* Configure routers
* Configure switches
* Simulate packet flow
* Learn networking

### Viva Answer

Packet Tracer allows us to create and test virtual networks without physical hardware.

---

# 25. What is a Default Gateway?

### Answer

Default Gateway is the IP address of the router used to send packets outside the local network.

### Example

PC:

```text
192.168.1.10
```

Gateway:

```text
192.168.1.1
```

### Working

If the destination is outside the local network, the PC forwards the packet to the gateway.

### Common Viva

**What happens if the gateway is wrong?**

The device can communicate within the LAN but cannot reach other networks or the Internet.

---

# 10 Questions Examiners Ask Immediately After These

### What is IPv4?

32-bit logical address.

### What is IPv6?

128-bit logical address.

### What is Loopback Address?

127.0.0.1

### What is a Port Number?

Logical endpoint used by applications.

### HTTP Port?

80

### HTTPS Port?

443

### DNS Port?

53

### FTP Port?

21

### SSH Port?

22

### Telnet Port?

23

---

If you memorize these 25 detailed answers plus the follow-up questions, you'll be prepared for the majority of CN practical viva discussions. The next level of preparation would be a **mock viva with 100+ examiner-style tricky questions and ideal answers**, which is often enough to handle unexpected viva questions confidently.






That's the best way to prepare. Since practical exams usually pick one experiment and then ask theory from the related unit, we'll cover each experiment in this format:

1. **Aim**
2. **Theory**
3. **Algorithm**
4. **Expected Output**
5. **How to Explain to Examiner**
6. **Viva Questions**
7. **Related Theory Questions from Syllabus**

---

# Experiment 1

# Study of LAN Using Different Network Topologies and Network Devices

## Aim

To study various network topologies and networking devices used in LAN.

---

# Theory

## What is LAN?

LAN (Local Area Network) is a network that connects devices within a limited geographical area such as:

* Classroom
* Office
* Laboratory
* Building

### Characteristics

* High speed
* Low latency
* Privately owned
* Low cost

---

# Network Topologies

A topology defines how devices are connected.

## 1. Bus Topology

![Image](https://images.openai.com/static-rsc-4/6ozVyOr5Eu2xQyWWtu0ujf_kpBH5PWMHgm8tJ4Fn3h9pxYFw5pA1zzrscDF1U6Dxl_MJ2rcAwhAUlKsfL4cLxyAXNEgor8LR3KEZJTNNAMIDB_WOnp9hDtAstB1Z4XGXID1zXlmc6rSLPx9iLwOU1Jzx_EOSFQQ-6FUYhiYYYscnouICfWYj-ZLCFFDpi8Bd?purpose=fullsize)

![Image](https://images.openai.com/static-rsc-4/07k0bzpXq-8-zC35yvo2D1VQjtcuF5izvGKoBIOTfjlhqbI6k8-3Ea-J1N1sG5G1AjySC9JyjkmNZDtVPg9ZaztA2INPIpbaCvmGFTlMNJu0CjmENEPHLl_QuNCO1I1_zyS_VsBco4CqcrIkLc1jYpu5laigUM5vZxBPiV_qPFhy_GvW0acCvN_azL5JV0_i?purpose=fullsize)

![Image](https://images.openai.com/static-rsc-4/tLww8-XwFo9t01Qo4SN6cBJoYzySXthu3Ry1lCKDVlk50nkNtE_fcAR62R1c74aO7jJGRnVEYg5xMQptFEn4LZyiOSYDi-qK9BPnNSeL7-Nnd4eb-l8u2G6iSFuodaKgN7_ognEYxNHE4PVtwa1Ow8dSyxpaCT7P9bC0Flvnydm56E8dgCggPMo15M-ZQuvp?purpose=fullsize)

![Image](https://images.openai.com/static-rsc-4/hzET0RnwBq7rcdY6NkczaKvVYxIl0Up7YkFE9CksPcE0U_AKGMMG8pCBfsgm7HjpFCEy4wF4nWSmpdTSeaK9SMlvZfvQptZCcLyAVSy9lDo08K33PJMMskkBwD2iidqY3oJPYsAMkelMsKsO3yRLyENUxyQN6-W6mFoa4CVDAfhkiy0a0wEUEJY3mVbMhdS6?purpose=fullsize)

![Image](https://images.openai.com/static-rsc-4/oDCEwYkz4uVPuXyY6OaEugw7jq05XRngAxUhXMO-0ldJI0Zk3tLpf-gjoBctO4dYUI7_yPrt278CrAWBc4YrNsO9ugQ_5dokuuPnP8H7ArgEwdfxeSnRfz0wPrQwqbKOJDCX5-QZ3naKgwI0fDIjUMeP8e24vks9ov1M0f-vAV_lQ8-MJtuIJojgAYqVOqnS?purpose=fullsize)

### Working

All computers share a common backbone cable.

### Advantages

* Cheap
* Easy installation

### Disadvantages

* Backbone failure affects whole network
* Difficult troubleshooting

---

## 2. Star Topology

![Image](https://images.openai.com/static-rsc-4/oo-iGyE__uNk5qDkaCXHvD2SZXDVnG4WLC1Q1hm3OE_s8BCuRaprxNr0QJpZA9tdY_Ep-z-FghdRyX-_8vn1yN0NweK-mZJwL1Jp0e3APfv_EDWOkdgqf_iiDjbPhq3o3COnj72DiouiosLiWWKmwzY3IJzKh8Gxq0NNwlg1WrZHJSs7KsKXxmjBkDAIA1yy?purpose=fullsize)

![Image](https://images.openai.com/static-rsc-4/q120XLVi5el2y3Btw2wMefOVb_3Q4CQiv1ti1labgUDm9PBSSgo8IYzzPtfMfwJ5n9MSy_FkHL7l3TAFk6h0eN1oYsqyg_zkO-ZHa01h3ZsXuG87aDMXnp98gnSINgcDY7eKMrD6CQB8zrEP38Jf0Pfm1uvDPdbvYIm9gPPuN_a1sbzE-uFXDAJ5_9toRJ6N?purpose=fullsize)

![Image](https://images.openai.com/static-rsc-4/CL7b8KwmE9KOcqL1cXI3P9ovP0U-11lgbG4SLcLgN3SK-kgawNhYb0kDBwMVA3zT1tXn2G6f5CH8muSBmwFC39lICGroFCF9kN5RFT5pzPmXBrBgAYOubu22praSoMKuJsoDdxUaJ8O6jHWDqy5Gt7GY9jYyJyGE-I59jAyFr4fo0_eWUbhS2cJ4zTIOUfz5?purpose=fullsize)

![Image](https://images.openai.com/static-rsc-4/DuhEhfobIfXJoEtbukXsFkuI9H2HsrOVFISiIyqeLAE18jh3J7iupvjqLCDmjg8oSFve5_gbKnGxpe7hMXavK1hsTkq-q096JmS4kAq3n-MYTAt_f7jNMceFcwQztkazsYXbEKhVnp5VcHYfnihbwZ-igFBAQPxDntTHJsxljjIWFvVEZLLkz-Mz5pBNc6x9?purpose=fullsize)

![Image](https://images.openai.com/static-rsc-4/J20Tetmcaq200fIengGzbmg5i-eJffTTKjPwfaLxludclZVq_7KG0aDD5LwLwwB5PaK-RJwQzS58SaPirrO6uAy0_CLAozLFJ2TcLXg2yz41syZfvTEuBOcRGyJD3-WfdDXadz37Dx4dGMReGb9pdn1L6I09DP4ANkkYCHic7QOQ7GOI1UWXi4tlfVg0DRW5?purpose=fullsize)

### Working

All devices connect to a central switch.

### Advantages

* Easy maintenance
* Fault isolation

### Disadvantages

* Switch failure affects network

### Most commonly used topology

**Star Topology**

---

## 3. Ring Topology

![Image](https://images.openai.com/static-rsc-4/9fyBv2s1BQMZdflg0L-GzVB9WwAN68q5JaDzFwAdCuoJH653EXstotXyPxQeYc-ztlt40DMDTgwCuTR0P4ELIa_-xQ7Kr8X7KxSOTlEIdl58REUnU1wnwWU4weu8wu6y82ZVzZKaJRl6mMKCNOlvEtwxXj7QpnzJREPTY_5YVUFJjsitIVkf6dqbsjnYhq4d?purpose=fullsize)

![Image](https://images.openai.com/static-rsc-4/2ayMvqeZLbMwKFl4d5svYN66JROnrV5zBwvgMCI6l890iA_egQVNm4gVeT7NT09hmEe7iEz9No9PMXOj-ml20Y4gDBgDMeGU_hAUpzFfO_4mw96kXDk7slcJdDXXibBMBJ9HCDvETYnQzWCVpIcQHxc9zzxF97AgG-CL5W0cmet4ufg9KmOrSFBRTEt4F-ob?purpose=fullsize)

![Image](https://images.openai.com/static-rsc-4/_ymxKMSR2gF5PRSFjKAZfDU8uagIRHNe_aCGz0QH9Bq-nL1XuXxjZp8Z2avBeqZTrBXfqICcGgI79LEjtWQc2ps27d069mocRV2gwlbkHNQASlLL04Fohua7LcWs0rNm-MorK0K1QIdnwihT8ixJzGf71Smu8TgDYoTXkjjvI0NGe1X3HQp203xqe8PgqBcN?purpose=fullsize)

![Image](https://images.openai.com/static-rsc-4/GP9iAsA8UJ4SxasddhbCWRV1-9xtjxPN5a7wG1-gU010Q9NHMaQ7omda8lnBJOXlabk9w06qnr2hNKHiXfu5GVihWg5GwL0ltJLATtecFG0quimVsDbE1WRFmGN2g4-JVb35YvUjE1BzjH7IuAB-nkfQ8Ugdz_2IPSN8p4PlDDekZ1BsAxEGDi2DBhXi3VIQ?purpose=fullsize)

### Working

Each node connects to two neighboring nodes.

Data moves in circular form.

### Uses

Token Passing

---

## 4. Mesh Topology

### Working

Every node connected to every other node.

### Formula

\frac{n(n-1)}{2}

Number of links required.

### Advantages

* Highly reliable
* Fault tolerant

### Disadvantages

* Expensive

---

# Network Devices

## Hub

### Layer

Physical Layer (Layer 1)

### Working

Broadcasts data to all devices.

### Problem

Collisions occur.

---

## Switch

### Layer

Data Link Layer (Layer 2)

### Working

Uses MAC address table.

Sends frame only to destination.

---

## Router

### Layer

Network Layer (Layer 3)

### Working

Uses IP addresses.

Connects different networks.

---

## Bridge

### Layer

Data Link Layer

Connects LAN segments.

---

## Repeater

### Layer

Physical Layer

Regenerates weak signals.

---

## Gateway

Works at multiple layers.

Used to connect different protocols.

---

# How to Explain to Examiner

> "LAN is a network connecting devices within a small geographical area. Different topologies define the arrangement of nodes. Star topology is the most widely used because of its easy maintenance and fault isolation. Network devices such as hubs, switches, routers, repeaters and gateways perform different functions at different OSI layers."

---

# Most Important Viva Questions

## Q1 What is LAN?

A local area network connecting devices within a limited area.

---

## Q2 Difference between LAN and WAN?

| LAN        | WAN        |
| ---------- | ---------- |
| Small area | Large area |
| Faster     | Slower     |
| Low cost   | Expensive  |

---

## Q3 Which topology is most commonly used?

Star topology.

---

## Q4 Which device works at Layer 2?

Switch

---

## Q5 Which device works at Layer 3?

Router

---

## Q6 Difference between Hub and Switch?

| Hub        | Switch                 |
| ---------- | ---------------------- |
| Broadcasts | Intelligent forwarding |
| Layer 1    | Layer 2                |
| Slow       | Fast                   |

---

## Q7 Why is Star topology preferred?

Easy troubleshooting and fault isolation.

---

## Q8 What is a collision?

When two devices transmit simultaneously.

---

## Q9 Which topology provides maximum reliability?

Mesh topology.

---

## Q10 What is a backbone cable?

Main cable used in Bus topology.

---

# Related Theory Questions from Unit 1

### What is Internet?

Global network of interconnected networks.

---

### Modes of Communication

#### Simplex

One-way

Example:
Keyboard → Computer

#### Half Duplex

Both directions but one at a time

Example:
Walkie-talkie

#### Full Duplex

Both directions simultaneously

Example:
Telephone

---

### Difference Between OSI and TCP/IP

| OSI             | TCP/IP          |
| --------------- | --------------- |
| 7 layers        | 4 layers        |
| Reference model | Practical model |
| ISO             | DARPA           |

---

### Physical Layer Responsibilities

* Transmission of bits
* Signal encoding
* Transmission media

---

### Guided Media

* Twisted Pair
* Coaxial
* Optical Fiber

---

### Unguided Media

* Radio Waves
* Microwave
* Infrared

---

### Switching Techniques

#### Circuit Switching

Dedicated path.

Example:
Telephone network.

#### Packet Switching

Data divided into packets.

Example:
Internet.

#### Message Switching

Entire message forwarded.

Store and forward.

---

# Examiner's Favorite Rapid-Fire Questions

1. How many layers in OSI?

   * 7

2. Which layer handles routing?

   * Network Layer

3. Which layer handles framing?

   * Data Link Layer

4. Which topology is used in offices?

   * Star

5. Device used to connect two networks?

   * Router

6. Which device forwards based on MAC address?

   * Switch

7. Which device forwards based on IP address?

   * Router

8. Which topology requires maximum cables?

   * Mesh

9. Which topology uses token passing?

   * Ring

10. Which device regenerates signals?

* Repeater

---

This single experiment alone covers almost **Unit 1 (Physical Layer)** and a portion of **Unit 2 (Data Link Layer)** viva.

Next, we should do **Experiment 2 (RJ45, CAT6, T568A/T568B, Crimping, Straight-through and Cross-over Cables)** because it is one of the most frequently asked practical and viva topics.



# Experiment 2

# Study of Networking Hardware, RJ-45 Connector, CAT-6 Cable, Crimping, Straight Cable, Cross Cable and Cable Testing

This is one of the **most important CN practicals** because examiners love asking viva from it.

---

# Aim

To study networking hardware and perform:

* RJ45 connector crimping
* Straight-through cable creation
* Cross-over cable creation
* Cable testing
* Understanding T568A and T568B standards

---

# Theory

## What is NIC?

### NIC (Network Interface Card)

A hardware component that allows a computer to connect to a network.

### Functions

* Provides MAC Address
* Enables communication with network

### Layer

Works mainly at:

* Physical Layer
* Data Link Layer

---

## What is RJ45 Connector?

RJ45 stands for:

**Registered Jack 45**

It is an 8-pin connector used in Ethernet networks.

![Image](https://images.openai.com/static-rsc-4/hXY-JJh49oHPe4iLOJT2Di2MBx15ksevk7fO6enGJw3VZVNOFdAzq7BEJSREtXopSMBGyoShsBY7s4t9ASRInH7RtI8bnqR-qKAwLoS27TGuf4dsPpp-Y8uGZ1vd7sRjP64Gre7odqHi-bGbg4U8YGdraI4SCYmmVbEglnHt6MIX8OOlXX6zZiFBvaM0xFWz?purpose=fullsize)

![Image](https://images.openai.com/static-rsc-4/t8iMTz71pDX93rS7Xo3pKZZQ7yIO886TlBpoXy_IZWfnV5hjq9ZfHziK-SJRp2ZaRZaB9yatb4-y4VdeLu0TIrQ0ZZkZKsGZ3oSh1ie67qOsYaKO2gOpMr09OrKXVyPg7qyUl7V4MKptk9PlTZQ4dSmT-mhtr0_pMrhPzqkhy05v1Qhzaw7WRARdlccqb5vz?purpose=fullsize)

![Image](https://images.openai.com/static-rsc-4/2TAalYcMPU-O_JhrYmKguwY4WIo2Zoqdq7GNy2BoZXq2xUK64ag3AzztWcjtQ9SrCdrIsA_VWpuVvoWss8QIDwcMBBAPbG6jaWs7QEkrtB2u6MpJsxEjPZlZMPZ5Qk43dwl2YaT1NuBs4RZSmwLul3V1Z6_uDe7xNnUJGYP1nu_zAxiWh-vcXxp4YJWsybIQ?purpose=fullsize)

![Image](https://images.openai.com/static-rsc-4/_RsCFVB_IkWcTgLzynW2bHGg_6KKu1B7LD_RxR9Joadf1_ZjdW2z0N9gkqZzNgZWdQytnnG7KCmV6eVAPlEakt9QiIZdFAtg7A2wUYb0YXaQvTAqO0OmP5ABs8Se0K0qiSOWYtHjZm1ph__UH2qM1Zdtuf7h19AK_Ir-w-YK8J5mOvjHD5wWfy6TgqeKvYmn?purpose=fullsize)

### Important Viva

Q. How many pins does RJ45 have?

Answer:

**8 Pins**

---

# CAT-6 Cable

CAT = Category

CAT-6 is a twisted pair Ethernet cable.

### Features

* Supports Gigabit Ethernet
* Less interference
* Higher speed than CAT5

### Speed

Up to:

```text
1 Gbps (commonly)
```

---

# Twisted Pair Cable

Pairs are twisted to reduce:

* Noise
* Crosstalk
* Electromagnetic interference

---

# Color Coding Standards

There are two standards:

1. T568A
2. T568B

---

# T568A Standard

Pin sequence:

| Pin | Color        |
| --- | ------------ |
| 1   | White-Green  |
| 2   | Green        |
| 3   | White-Orange |
| 4   | Blue         |
| 5   | White-Blue   |
| 6   | Orange       |
| 7   | White-Brown  |
| 8   | Brown        |

---

# T568B Standard

Pin sequence:

| Pin | Color        |
| --- | ------------ |
| 1   | White-Orange |
| 2   | Orange       |
| 3   | White-Green  |
| 4   | Blue         |
| 5   | White-Blue   |
| 6   | Green        |
| 7   | White-Brown  |
| 8   | Brown        |

---

# IMPORTANT MEMORY TRICK

### T568B

```text
WO O WG B WB G WB Br
```

Where:

WO = White Orange

WG = White Green

WB = White Blue

Br = Brown

Most labs use **T568B**.

---

# Straight Through Cable

## Definition

Both ends use same standard.

Example:

```text
T568B -------- T568B
```

OR

```text
T568A -------- T568A
```

---

# Uses

Connect:

* PC → Switch
* PC → Hub
* Switch → Router

---

# Cross Over Cable

## Definition

One end T568A

Other end T568B

```text
T568A ------- T568B
```

---

# Uses

Connect similar devices:

* PC → PC
* Switch → Switch
* Hub → Hub

---

# Why Called Cross Cable?

Transmit and Receive pairs are crossed.

Specifically:

```text
Pin 1 ↔ Pin 3
Pin 2 ↔ Pin 6
```

---

# Crimping Process

## Step 1

Cut CAT6 cable.

---

## Step 2

Remove outer insulation.

---

## Step 3

Separate twisted pairs.

---

## Step 4

Arrange colors according to standard.

---

## Step 5

Trim evenly.

---

## Step 6

Insert wires into RJ45.

---

## Step 7

Use crimping tool.

---

## Step 8

Verify with cable tester.

---

# Cable Tester

Purpose:

Check cable continuity.

Detect:

* Open circuit
* Short circuit
* Wrong sequence

---

# How Cable Tester Works

LEDs glow sequentially:

```text
1 2 3 4 5 6 7 8
```

If sequence is correct:

Cable is good.

---

# How to Explain Practical to Examiner

> "In this experiment we study networking hardware and prepare Ethernet cables using RJ45 connectors. We arrange wires according to T568A or T568B standard, insert them into RJ45 connectors and use a crimping tool to make proper contact. Finally, we verify the cable using a cable tester."

---

# Very Important Viva Questions

## Q1 What is RJ45?

An 8-pin Ethernet connector.

---

## Q2 Why are twisted pairs used?

To reduce noise and crosstalk.

---

## Q3 What is CAT6?

Category 6 Ethernet cable used for high-speed networking.

---

## Q4 What is crimping?

Attaching RJ45 connector to Ethernet cable.

---

## Q5 Difference Between Straight and Cross Cable?

| Straight                | Cross               |
| ----------------------- | ------------------- |
| Same standard both ends | Different standards |
| PC-Switch               | PC-PC               |

---

## Q6 Which pins are crossed?

```text
1 ↔ 3
2 ↔ 6
```

---

## Q7 Which cable is used between PC and Switch?

Straight-through cable.

---

## Q8 Which cable is used between Switch and Switch?

Cross-over cable.

---

## Q9 How many twisted pairs are in CAT6?

4 pairs.

---

## Q10 How many wires are inside Ethernet cable?

8 wires.

---

## Q11 What is Crosstalk?

Signal interference between wire pairs.

---

## Q12 What is attenuation?

Signal strength reduction over distance.

---

## Q13 What is the maximum length of Ethernet cable?

```text
100 meters
```

Very frequently asked.

---

## Q14 What is MAC Address?

48-bit physical address assigned to NIC.

Example:

```text
00:1A:2B:3C:4D:5E
```

---

## Q15 Which layer uses MAC Address?

Data Link Layer

---

# Related Theory Questions (Unit 1 + Unit 2)

## Transmission Media

### Guided Media

* Twisted Pair
* Coaxial
* Optical Fiber

---

### Unguided Media

* Radio
* Microwave
* Infrared

---

# Fiber Optic Cable

Advantages:

* Very high speed
* Long distance
* Immune to EMI

---

# Coaxial Cable

Used in:

* Cable TV
* Broadband

---

# Data Link Layer Functions

1. Framing
2. Error Control
3. Flow Control
4. Access Control

---

# Ethernet Standard

IEEE:

```text
802.3
```

---

# WiFi Standard

IEEE:

```text
802.11
```

---

# Bluetooth Standard

IEEE:

```text
802.15
```

---

# Quick 1-Mark Questions

### Which cable is mostly used today?

CAT6

---

### Connector used in Ethernet?

RJ45

---

### Number of pins in RJ45?

8

---

### Number of twisted pairs?

4

---

### Device connecting host to network?

NIC

---

### Ethernet works on which topology?

Star

---

### Standard Ethernet IEEE?

802.3

---

### WiFi IEEE?

802.11

---

### Maximum Ethernet cable length?

100 meters

---

### Layer responsible for framing?

Data Link Layer

---

# What Examiners Often Ask After This Experiment

Immediately after cable questions, they often jump to:

1. `ipconfig`
2. `ping`
3. `tracert`
4. `nslookup`
5. `arp -a`
6. DNS
7. MAC Address
8. IP Address

These belong to **Experiment 3**, which is another extremely high-probability practical and viva topic.

**Next: Experiment 3 — Networking Commands (ipconfig, ping, tracert, nslookup, telnet, ftp, arp, netstat) in complete detail with outputs, packet flow, and viva questions.**



# Experiment 3

# Running and Using Networking Commands (ipconfig, ping, tracert, nslookup, telnet, ftp, arp, netstat)

This is one of the **most commonly assigned CN practicals** because it directly relates to real networking.

---

# Aim

To study and use various networking commands for:

* Network configuration
* Connectivity testing
* Route tracing
* DNS lookup
* ARP table inspection
* Active connection monitoring

---

# Why This Practical Is Important

When you perform:

```bash
ping google.com
```

You are actually using concepts from:

* Physical Layer
* Data Link Layer
* Network Layer
* Transport Layer
* Application Layer

Therefore viva can come from the entire syllabus.

---

# Command 1: ipconfig

## Purpose

Displays IP configuration of a system.

---

## Command

```cmd
ipconfig
```

---

## Output

```text
IPv4 Address : 192.168.1.10
Subnet Mask  : 255.255.255.0
Default Gateway : 192.168.1.1
```

---

# Important Terms

## IPv4 Address

Logical address of device.

Example:

```text
192.168.1.10
```

---

## Subnet Mask

Defines network and host portion.

Example:

```text
255.255.255.0
```

---

## Default Gateway

Router address used to reach outside networks.

Example:

```text
192.168.1.1
```

---

# Viva Questions

### Q. What does ipconfig do?

Displays IP configuration.

---

### Q. What is default gateway?

Router address through which packets leave the network.

---

### Q. What is subnet mask?

Separates network and host portions.

---

# Command 2: ping

## Purpose

Checks connectivity between two devices.

---

## Command

```cmd
ping google.com
```

---

## Example Output

```text
Reply from 142.250.x.x
time=25ms
TTL=117
```

---

# How Ping Works

Uses:

**ICMP Protocol**

(Network Layer)

---

# Meaning of TTL

TTL = Time To Live

Prevents packets from circulating forever.

Every router decreases TTL by 1.

---

# Meaning of Time

Latency between source and destination.

---

# Viva Questions

### Q. Which protocol is used by ping?

ICMP

---

### Q. Which layer handles ICMP?

Network Layer

---

### Q. What is TTL?

Time To Live

---

### Q. What if ping request times out?

Destination unreachable or blocked.

---

# Command 3: tracert

(Traceroute)

---

## Purpose

Shows route taken by packet.

---

## Command

```cmd
tracert google.com
```

---

## Example

```text
1 Router
2 ISP Router
3 ISP Core Router
4 Google Server
```

---

# Working

Uses:

* ICMP
* TTL values

Each router decreases TTL.

When TTL becomes zero:

Router sends ICMP Time Exceeded message.

---

# Viva Questions

### Q. Why use tracert?

To identify route and delays.

---

### Q. Which protocol does tracert use?

ICMP

---

### Q. What is a hop?

A router between source and destination.

---

# Command 4: nslookup

## Purpose

DNS lookup.

Converts:

```text
Domain Name → IP Address
```

---

## Command

```cmd
nslookup google.com
```

---

## Example Output

```text
Name: google.com
Address: 142.250.x.x
```

---

# Working

Queries DNS server.

---

# Viva Questions

### Q. What is DNS?

Domain Name System.

---

### Q. Why is DNS needed?

Humans remember names better than IPs.

---

### Q. Which port does DNS use?

53

---

### Q. Which transport protocol does DNS use?

Usually UDP.

Sometimes TCP.

---

# Command 5: arp -a

## Purpose

Displays ARP cache.

---

## Command

```cmd
arp -a
```

---

## Example

```text
192.168.1.1
00-AA-BB-CC-DD-EE
```

---

# What is ARP?

ARP = Address Resolution Protocol

Converts:

```text
IP Address → MAC Address
```

---

# Working

Suppose:

```text
IP = 192.168.1.20
```

Computer asks:

> "Who owns this IP?"

Owner replies with MAC address.

---

# Viva Questions

### Q. Full form of ARP?

Address Resolution Protocol

---

### Q. ARP converts?

IP to MAC

---

### Q. Layer of ARP?

Works between Layer 2 and Layer 3.

---

# Command 6: netstat

## Purpose

Displays active network connections.

---

## Command

```cmd
netstat
```

---

## Output

```text
TCP
UDP
Local Address
Foreign Address
State
```

---

# States

## LISTENING

Waiting for connection.

---

## ESTABLISHED

Connection active.

---

## CLOSE_WAIT

Waiting to close connection.

---

# Viva Questions

### Q. What does netstat show?

Active network connections.

---

### Q. What is LISTENING state?

Waiting for incoming connection.

---

### Q. What is ESTABLISHED state?

Connection successfully formed.

---

# Command 7: telnet

## Purpose

Remote login protocol.

---

## Command

```cmd
telnet hostname
```

---

# Port Number

```text
23
```

---

# Problems

* No encryption
* Insecure

---

# Modern Replacement

SSH

---

# Viva Questions

### Q. Why is Telnet insecure?

Data sent in plain text.

---

### Q. Which protocol replaced Telnet?

SSH

---

### Q. Telnet port number?

23

---

# Command 8: FTP

## Purpose

File Transfer Protocol.

---

## Uses

Transfer files between systems.

---

# Port Number

```text
21
```

---

# FTP Modes

### Active Mode

Server initiates data connection.

---

### Passive Mode

Client initiates connection.

---

# Viva Questions

### Q. Full form of FTP?

File Transfer Protocol

---

### Q. FTP Port Number?

21

---

### Q. Secure version of FTP?

SFTP

---

# Theory Behind These Commands

These commands touch multiple syllabus topics.

---

# IP Addressing

## IPv4

32-bit address.

Example:

```text
192.168.1.10
```

---

## IPv6

128-bit address.

Example:

```text
2001:db8::1
```

---

# Classful Addressing

## Class A

```text
1-126
```

Default Mask:

```text
255.0.0.0
```

---

## Class B

```text
128-191
```

Default Mask:

```text
255.255.0.0
```

---

## Class C

```text
192-223
```

Default Mask:

```text
255.255.255.0
```

---

## Class D

```text
224-239
```

Multicasting

---

## Class E

```text
240-255
```

Experimental

---

# Frequently Asked Port Numbers

| Service | Port |
| ------- | ---- |
| HTTP    | 80   |
| HTTPS   | 443  |
| FTP     | 21   |
| SSH     | 22   |
| Telnet  | 23   |
| SMTP    | 25   |
| DNS     | 53   |

**Memorize these.**

---

# Extremely Common Viva Questions

### Q. Difference between MAC and IP?

| MAC              | IP              |
| ---------------- | --------------- |
| Physical Address | Logical Address |
| Layer 2          | Layer 3         |
| Permanent        | Can change      |

---

### Q. What is a packet?

Unit of data at Network Layer.

---

### Q. What is a frame?

Unit of data at Data Link Layer.

---

### Q. What is a segment?

Unit of data at Transport Layer.

---

### Q. Which command tests connectivity?

ping

---

### Q. Which command traces route?

tracert

---

### Q. Which command resolves domain names?

nslookup

---

### Q. Which command shows MAC mappings?

arp -a

---

### Q. Which command displays active connections?

netstat

---

# Examiner's Trap Questions

### If ping works but website does not open, what could be wrong?

DNS problem.

---

### If nslookup fails?

DNS server issue.

---

### If tracert stops at a router?

Network issue beyond that router.

---

### If default gateway is wrong?

Internet won't work.

---

# How to Explain This Practical in 30 Seconds

> "In this experiment we use networking commands such as ipconfig, ping, tracert, nslookup, arp and netstat. These commands help us view IP configuration, test connectivity, trace packet routes, resolve domain names, inspect ARP mappings and monitor active network connections. They are useful for network troubleshooting and administration."

---

This experiment covers a large part of **Unit 3 (Network Layer)** and some **Application Layer** concepts.

Next comes **Experiment 4: Establish a Physical Peer-to-Peer Network Connection using NICs, Cables, Switch and Router**, which usually leads to viva on LAN, IP addressing, switches, routers, ARP, DHCP and packet flow.




# Experiment 4

# Establish a Physical Peer-to-Peer Network Connection Using NIC, Cables, Switch and Router

This experiment is extremely important because it combines **practical networking hardware** with **Network Layer concepts**. Examiners often ask packet-flow questions from this experiment.

---

# Aim

To establish communication between two or more computers using:

* NIC (Network Interface Card)
* Ethernet Cable
* Switch
* Router

and verify connectivity using network commands.

---

# Theory

## What is Peer-to-Peer Network?

A Peer-to-Peer (P2P) network is a network where computers communicate directly and can act as both:

* Client
* Server

No dedicated server is required.

---

## Example

Two PCs connected directly.

```text
PC1  <------->  PC2
```

Both can share:

* Files
* Printers
* Data

---

# Types of Physical Connection

## Direct Connection

```text
PC1 -------- PC2
```

Uses:

Cross-over Cable

---

## Connection Through Switch

```text
PC1
     \
      Switch
     /
PC2
```

Uses:

Straight-through Cable

---

## Connection Through Router

```text
PC1 ---- Router ---- PC2
```

Used when devices belong to different networks.

---

# Hardware Used

## NIC (Network Interface Card)

Purpose:

Connects computer to network.

Provides:

* MAC Address
* Physical connection

---

### Important Viva

Q. What is the length of MAC Address?

Answer:

```text
48 bits
```

Example:

```text
00:1A:2B:3C:4D:5E
```

---

# Ethernet Cable

Used for physical transmission.

Usually:

CAT5e or CAT6

---

# Switch

Layer:

Data Link Layer (Layer 2)

Uses:

MAC Address Table

---

# Router

Layer:

Network Layer (Layer 3)

Uses:

IP Addresses

Purpose:

Connects different networks.

---

# Procedure

## Step 1

Connect PCs using switch.

```text
PC1 ---- Switch ---- PC2
```

---

## Step 2

Assign IP Addresses.

Example:

### PC1

```text
192.168.1.10
```

---

### PC2

```text
192.168.1.20
```

---

### Subnet Mask

```text
255.255.255.0
```

for both.

---

## Step 3

Check configuration.

```cmd
ipconfig
```

---

## Step 4

Verify connectivity.

```cmd
ping 192.168.1.20
```

---

## Step 5

Successful reply indicates connection established.

---

# How Communication Happens

Suppose:

```text
PC1 → PC2
```

---

## Step 1

Application generates data.

---

## Step 2

Transport Layer creates segment.

---

## Step 3

Network Layer adds IP Address.

---

## Step 4

Data Link Layer adds MAC Address.

---

## Step 5

Frame reaches Switch.

---

## Step 6

Switch checks MAC Table.

---

## Step 7

Switch forwards frame.

---

## Step 8

PC2 receives data.

---

# Packet Flow (Very Important Viva)

Examiner may ask:

> "What happens when you ping another PC?"

Answer:

1. Source checks ARP cache.
2. If MAC not found, ARP Request is broadcast.
3. Destination replies with ARP Reply.
4. ICMP Echo Request sent.
5. Destination sends ICMP Echo Reply.
6. Ping successful.

This answer alone impresses most examiners.

---

# ARP Process

ARP = Address Resolution Protocol

Converts:

```text
IP Address → MAC Address
```

---

## Example

PC1 wants:

```text
192.168.1.20
```

but only knows IP.

It broadcasts:

```text
Who has 192.168.1.20?
```

PC2 replies:

```text
I have 192.168.1.20
My MAC is 00-AA-BB-CC-DD
```

---

# DHCP

Another favorite viva topic.

---

## DHCP

Dynamic Host Configuration Protocol

Automatically provides:

* IP Address
* Subnet Mask
* Gateway
* DNS

---

## DHCP Port Numbers

Server:

```text
67
```

Client:

```text
68
```

---

## DHCP Process

DORA

### D

Discover

---

### O

Offer

---

### R

Request

---

### A

Acknowledge

---

# Static IP vs Dynamic IP

| Static           | Dynamic       |
| ---------------- | ------------- |
| Manual           | Automatic     |
| Fixed            | Changes       |
| Admin configured | DHCP assigned |

---

# Difference Between Switch and Router

| Switch       | Router             |
| ------------ | ------------------ |
| Layer 2      | Layer 3            |
| MAC Address  | IP Address         |
| Same Network | Different Networks |

---

# How to Explain Practical

> "In this experiment we establish a peer-to-peer network using Ethernet cables, NICs and a switch. We assign IP addresses to systems, verify connectivity using ping, and observe how packets travel using MAC and IP addressing. ARP is used to obtain destination MAC addresses before communication begins."

---

# Most Important Viva Questions

## Q1 What is Peer-to-Peer Network?

A network where all computers act as equals.

---

## Q2 What is Client-Server Network?

A network with dedicated server providing services.

---

## Q3 Which cable connects PC to Switch?

Straight-through cable.

---

## Q4 Which cable connects PC to PC?

Cross-over cable.

---

## Q5 Why is IP Address required?

For logical identification.

---

## Q6 Why is MAC Address required?

For local delivery inside LAN.

---

## Q7 What is ARP?

Protocol converting IP to MAC.

---

## Q8 Which protocol is used by Ping?

ICMP

---

## Q9 What is DHCP?

Automatic IP allocation protocol.

---

## Q10 Full form of NIC?

Network Interface Card.

---

## Q11 What is a Default Gateway?

Router address used to reach other networks.

---

## Q12 What if two systems have same IP?

IP Conflict occurs.

Communication fails.

---

## Q13 What is a Collision Domain?

Area where packet collisions may occur.

Hub → One collision domain.

Switch → Separate collision domains.

---

## Q14 What is a Broadcast Domain?

Group receiving broadcast packets.

Routers separate broadcast domains.

---

## Q15 Why is Switch better than Hub?

Switch sends frames only to intended destination.

---

# Related Theory Questions (Unit 2 & Unit 3)

## Data Link Layer Functions

1. Framing
2. Error Control
3. Flow Control
4. Access Control

---

## Network Layer Functions

1. Routing
2. Logical Addressing
3. Packet Forwarding

---

## IPv4

Length:

```text
32 bits
```

---

## IPv6

Length:

```text
128 bits
```

---

## NAT

Network Address Translation

Converts:

```text
Private IP → Public IP
```

---

## Private IP Ranges

Class A:

```text
10.0.0.0 – 10.255.255.255
```

Class B:

```text
172.16.0.0 – 172.31.255.255
```

Class C:

```text
192.168.0.0 – 192.168.255.255
```

---

# Examiner's Favorite Scenario Question

### Suppose PC1 can ping Router but cannot ping Google. Why?

Possible reasons:

1. DNS issue
2. ISP issue
3. Internet outage
4. Gateway misconfiguration

---

### Suppose ping by IP works but website does not open?

Answer:

DNS issue.

---

### Suppose ARP fails?

Source cannot obtain MAC address and communication cannot start.

---

# Quick Revision (Must Memorize)

| Term            | Answer                  |
| --------------- | ----------------------- |
| NIC             | Network Interface Card  |
| MAC Length      | 48 bits                 |
| IPv4 Length     | 32 bits                 |
| IPv6 Length     | 128 bits                |
| Ping Protocol   | ICMP                    |
| ARP             | IP → MAC                |
| DHCP            | Automatic IP assignment |
| Switch Layer    | Layer 2                 |
| Router Layer    | Layer 3                 |
| PC-Switch Cable | Straight                |
| PC-PC Cable     | Cross                   |

---

This experiment strongly covers **Network Layer, ARP, DHCP, MAC Addressing, IP Addressing, Switching and Routing**.

The next experiment is **Experiment 5: Wireshark Installation, Packet Capture and Traffic Analysis**, which is one of the highest-viva-weightage experiments because examiners can ask questions from **TCP, UDP, HTTP, DNS, ICMP, ARP, OSI Model, Encapsulation, and Protocol Analysis**.





# Experiment 5

# Installation and Use of Wireshark for Packet Capture and Analysis

This is one of the **highest-scoring CN practicals** because the examiner can ask questions from almost every layer of the OSI model.

---

# Aim

To install Wireshark, capture network packets, and analyze various protocols such as:

* ARP
* ICMP
* DNS
* TCP
* UDP
* HTTP
* HTTPS

---

# What is Wireshark?

## Definition

Wireshark is a **Network Protocol Analyzer**.

It captures packets traveling through a network interface and allows us to inspect them.

---

## Uses

* Troubleshooting
* Network monitoring
* Security analysis
* Protocol study
* Performance analysis

---

## Important Viva

### Q. What is Wireshark?

A packet capturing and protocol analysis tool.

---

### Q. Why is Wireshark used?

To capture and analyze network traffic.

---

# Installation

1. Download Wireshark
2. Install Npcap (important)
3. Launch Wireshark
4. Select network interface
5. Start capturing

---

# Network Interfaces

Examples:

* Ethernet
* Wi-Fi
* Loopback

Wireshark captures packets from the selected interface.

---

# Procedure

## Step 1

Open Wireshark.

---

## Step 2

Select active interface.

Example:

```text
Wi-Fi
```

or

```text
Ethernet
```

---

## Step 3

Start packet capture.

---

## Step 4

Generate traffic.

Example:

```cmd
ping google.com
```

---

## Step 5

Stop capture.

---

## Step 6

Analyze packets.

---

# Wireshark Window Sections

## Packet List Pane

Displays all captured packets.

---

## Packet Details Pane

Shows protocol hierarchy.

Example:

```text
Frame
Ethernet
IP
ICMP
```

---

## Packet Bytes Pane

Displays raw packet data.

---

# Packet Structure

Suppose:

```cmd
ping google.com
```

Captured packet:

```text
Ethernet
IP
ICMP
```

---

# Encapsulation (Very Important)

When data is sent:

Application Data

↓

TCP/UDP Header Added

↓

IP Header Added

↓

MAC Header Added

↓

Frame Sent

---

# Encapsulation Diagram

```text
+------------------+
| Application Data |
+------------------+

+------------------+
| TCP Header       |
| Application Data |
+------------------+

+------------------+
| IP Header        |
| TCP Header       |
| Application Data |
+------------------+

+------------------+
| MAC Header       |
| IP Header        |
| TCP Header       |
| Application Data |
+------------------+
```

---

# De-encapsulation

Reverse process at receiver.

---

# Important Protocols Seen in Wireshark

---

# ARP Packets

Filter:

```text
arp
```

---

## Purpose

Converts:

```text
IP → MAC
```

---

### Example

```text
Who has 192.168.1.1?
Tell 192.168.1.10
```

---

# ARP Packet Fields

* Source MAC
* Destination MAC
* Sender IP
* Target IP

---

# Viva Questions

### Q. Full form of ARP?

Address Resolution Protocol

---

### Q. Purpose of ARP?

IP to MAC mapping.

---

# ICMP Packets

Filter:

```text
icmp
```

---

## Generated By

```cmd
ping
```

---

### Types

#### Echo Request

Sent by source.

---

#### Echo Reply

Sent by destination.

---

# Viva Questions

### Q. Which protocol does ping use?

ICMP

---

### Q. Which layer handles ICMP?

Network Layer

---

# DNS Packets

Filter:

```text
dns
```

---

## Purpose

Domain Name Resolution

Example:

```text
google.com
```

↓

```text
142.250.x.x
```

---

# DNS Port

```text
53
```

---

# Viva Questions

### Q. Full form of DNS?

Domain Name System

---

### Q. Why DNS?

Converts names into IP addresses.

---

# TCP Packets

Filter:

```text
tcp
```

---

# TCP Features

* Reliable
* Connection-oriented
* Error recovery
* Acknowledgement

---

# TCP Three-Way Handshake

Extremely Important Viva

---

## Step 1

Client sends:

```text
SYN
```

---

## Step 2

Server sends:

```text
SYN ACK
```

---

## Step 3

Client sends:

```text
ACK
```

---

## Connection Established

```text
SYN
 ↓
SYN ACK
 ↓
ACK
```

---

# TCP Flags

| Flag | Meaning         |
| ---- | --------------- |
| SYN  | Synchronize     |
| ACK  | Acknowledgement |
| FIN  | Finish          |
| RST  | Reset           |
| PSH  | Push            |
| URG  | Urgent          |

---

# Viva Questions

### Q. Why TCP is reliable?

Uses acknowledgements and retransmissions.

---

### Q. Explain Three-Way Handshake.

SYN → SYN ACK → ACK

---

### Q. Which layer handles TCP?

Transport Layer

---

# UDP Packets

Filter:

```text
udp
```

---

# Features

* Connectionless
* Fast
* No ACK

---

# Uses

* Gaming
* Streaming
* DNS

---

# Viva Questions

### Q. Difference between TCP and UDP?

| TCP      | UDP        |
| -------- | ---------- |
| Reliable | Unreliable |
| ACK      | No ACK     |
| Slow     | Fast       |

---

# HTTP Packets

Filter:

```text
http
```

---

## Port

```text
80
```

---

# HTTP Methods

### GET

Fetch data.

---

### POST

Send data.

---

### PUT

Update.

---

### DELETE

Remove.

---

# Viva Questions

### Q. Full form of HTTP?

HyperText Transfer Protocol

---

### Q. Port Number?

80

---

# HTTPS

Port:

```text
443
```

---

# Difference

| HTTP       | HTTPS     |
| ---------- | --------- |
| Unsecured  | Secured   |
| Plain Text | Encrypted |
| Port 80    | Port 443  |

---

# IP Packet Analysis

Wireshark shows:

* Source IP
* Destination IP
* TTL
* Protocol

---

# TTL

Time To Live

Prevents routing loops.

Each router decreases TTL by 1.

---

# MAC Address Analysis

Wireshark displays:

```text
Source MAC
Destination MAC
```

---

# MAC Address Length

```text
48 bits
```

---

# IPv4 Address Length

```text
32 bits
```

---

# IPv6 Address Length

```text
128 bits
```

---

# Common Wireshark Filters

| Filter               | Purpose      |
| -------------------- | ------------ |
| arp                  | ARP packets  |
| icmp                 | Ping packets |
| dns                  | DNS packets  |
| tcp                  | TCP packets  |
| udp                  | UDP packets  |
| http                 | HTTP packets |
| ip.addr==192.168.1.1 | Specific IP  |
| tcp.port==80         | HTTP traffic |

**Memorize these.**

---

# How to Explain Practical to Examiner

> "In this experiment, Wireshark is used to capture and analyze packets travelling through a network interface. We observe protocols such as ARP, ICMP, DNS, TCP and HTTP. Packet headers reveal source and destination addresses, protocol information, ports and control flags. Wireshark helps in troubleshooting and understanding protocol operation."

---

# Most Important Viva Questions

### Q1 What is packet sniffing?

Capturing network packets.

---

### Q2 What is protocol analyzer?

A tool used to inspect network traffic.

---

### Q3 Why is Wireshark called a packet analyzer?

Because it captures and decodes packets.

---

### Q4 Which protocol resolves domain names?

DNS

---

### Q5 Which protocol is used by ping?

ICMP

---

### Q6 What is ARP used for?

IP to MAC conversion.

---

### Q7 Which protocol establishes reliable communication?

TCP

---

### Q8 Which protocol is faster?

UDP

---

### Q9 Which protocol uses Three-Way Handshake?

TCP

---

### Q10 What is TTL?

Time To Live.

---

### Q11 Which protocol secures websites?

HTTPS

---

### Q12 What is packet encapsulation?

Adding protocol headers at each layer.

---

### Q13 What is de-encapsulation?

Removing headers at receiver side.

---

### Q14 What is a port number?

Logical communication endpoint.

---

### Q15 Why are port numbers required?

To identify services and applications.

---

# Examiner's Favorite Rapid-Fire Questions

| Question      | Answer            |
| ------------- | ----------------- |
| Ping Protocol | ICMP              |
| DNS Port      | 53                |
| HTTP Port     | 80                |
| HTTPS Port    | 443               |
| FTP Port      | 21                |
| SSH Port      | 22                |
| Telnet Port   | 23                |
| SMTP Port     | 25                |
| TCP Reliable? | Yes               |
| UDP Reliable? | No                |
| IPv4 Length   | 32 bits           |
| IPv6 Length   | 128 bits          |
| MAC Length    | 48 bits           |
| ARP Function  | IP → MAC          |
| TCP Handshake | SYN, SYN-ACK, ACK |

---

# What Usually Comes Next in CN Labs

After Wireshark, labs generally move to:

### Experiment 6

**Study and Implementation of CRC (Cyclic Redundancy Check)**

This is one of the most frequently assigned programming practicals and often carries the toughest viva because examiners ask about:

* Error Detection
* Error Correction
* Hamming Distance
* CRC
* Parity Check
* Checksum
* Framing
* Data Link Layer

This experiment belongs directly to **Unit 2 (Data Link Layer)** and is extremely important for both practical and viva.



# Experiment 6

# Implementation of CRC (Cyclic Redundancy Check)

⚠️ **This is one of the most important CN practicals.**

If you get a programming experiment in CN practical, CRC is among the most probable.

Examiners also love asking CRC viva because it covers:

* Data Link Layer
* Error Detection
* Error Control
* Framing
* Transmission Errors

---

# Aim

To implement CRC (Cyclic Redundancy Check) for detecting transmission errors in data communication.

---

# Why CRC is Needed

During transmission:

```text
Sender --------> Receiver
```

Noise may change bits.

Example:

Original:

```text
1011001
```

Received:

```text
1010001
```

Error occurred.

CRC helps detect such errors.

---

# Theory

## Full Form

CRC = Cyclic Redundancy Check

It is an error detection technique used in:

* Ethernet
* Wi-Fi
* Data Link Layer protocols
* Storage devices

---

# Basic Idea

Sender:

1. Generates CRC bits
2. Appends them to data
3. Sends data

Receiver:

1. Performs same calculation
2. Checks remainder

If:

```text
Remainder = 0
```

No error.

Otherwise:

```text
Error detected
```

---

# Key Terms

## Dataword

Actual message.

Example:

```text
1101011011
```

---

## Generator Polynomial

Divisor used in CRC.

Example:

```text
10011
```

---

## Codeword

Data + CRC bits

---

# CRC Process

Suppose:

Data:

```text
1101011011
```

Generator:

```text
10011
```

Length of generator:

```text
5
```

Degree:

```text
4
```

---

# Step 1

Append 4 zeros.

```text
1101011011 0000
```

---

# Step 2

Perform Modulo-2 Division

( XOR Division )

Important:

No borrow
No carry

Rules:

```text
0 XOR 0 = 0
1 XOR 1 = 0
0 XOR 1 = 1
1 XOR 0 = 1
```

---

# Step 3

Get Remainder

Example:

```text
1110
```

---

# Step 4

Append Remainder

```text
1101011011 1110
```

This becomes transmitted codeword.

---

# Receiver Side

Receiver divides received codeword by same generator.

If:

```text
Remainder = 0000
```

Accepted.

Else:

```text
Error detected.
```

---

# Why XOR is Used?

Because CRC performs polynomial division over GF(2).

In binary arithmetic:

Addition = XOR

Therefore CRC uses XOR operations.

---

# Algorithm

### Sender

1. Read data.
2. Read generator.
3. Append zeros.
4. Perform XOR division.
5. Obtain remainder.
6. Append remainder.
7. Transmit codeword.

---

### Receiver

1. Receive codeword.
2. Divide by generator.
3. Check remainder.
4. If remainder is zero:

   * No error
5. Else:

   * Error detected

---

# How to Explain Program to Examiner

> "CRC is an error detection mechanism. The sender appends zeros equal to the degree of the generator polynomial and performs modulo-2 division using XOR operations. The obtained remainder is attached to the original data. At the receiver side the same division is performed. A non-zero remainder indicates transmission error."

This explanation is usually enough to get full practical marks.

---

# Modulo-2 Division

Most asked viva question.

---

### Q. What is Modulo-2 Division?

Binary division using XOR instead of subtraction.

---

### Q. Is carry used?

No.

---

### Q. Is borrow used?

No.

---

# Example Viva Calculation

Data:

```text
1011
```

Generator:

```text
11
```

Ask:

What is:

```text
1 XOR 1
```

Answer:

```text
0
```

---

### What is

```text
1 XOR 0
```

Answer:

```text
1
```

---

# Error Detection Techniques

Examiner often expands CRC viva into this topic.

---

## 1. Parity Check

Simplest method.

---

### Even Parity

Total number of 1s must be even.

Example:

```text
1011001
```

1s count:

```text
4
```

Already even.

Parity bit:

```text
0
```

---

### Odd Parity

Total number of 1s must be odd.

---

# Limitation

Can detect only some errors.

---

# 2. Checksum

Used in:

* TCP
* UDP
* IP

---

### Working

Data blocks added together.

Complement stored.

Receiver verifies.

---

# 3. CRC

Most powerful among these.

Can detect:

* Single-bit errors
* Double-bit errors
* Burst errors

---

# Why CRC is Better?

Because it detects burst errors effectively.

---

# Burst Error

Multiple consecutive bits corrupted.

Example:

Original:

```text
1011110101
```

Received:

```text
1010000101
```

Many bits changed together.

---

# Important Viva Questions

## Q1 Full Form of CRC?

Cyclic Redundancy Check

---

## Q2 Why CRC is used?

Error detection.

---

## Q3 Which layer uses CRC?

Data Link Layer

---

## Q4 What arithmetic is used in CRC?

Modulo-2 arithmetic.

---

## Q5 Which operation is used?

XOR

---

## Q6 What is Generator Polynomial?

Divisor used in CRC calculation.

---

## Q7 Why append zeros before division?

To create space for CRC bits.

---

## Q8 How many zeros are appended?

Degree of generator polynomial.

---

Example:

Generator:

```text
10011
```

Length = 5

Degree = 4

Append:

```text
0000
```

---

## Q9 What happens at receiver side?

Same division performed.

---

## Q10 What indicates error?

Non-zero remainder.

---

## Q11 What indicates no error?

Zero remainder.

---

## Q12 Difference Between CRC and Parity?

| CRC                  | Parity                          |
| -------------------- | ------------------------------- |
| Strong               | Weak                            |
| Detects burst errors | Cannot detect many burst errors |
| More reliable        | Less reliable                   |

---

## Q13 What is Hamming Distance?

Number of bit positions that differ.

Example:

```text
1011
1001
```

Difference:

1 bit

Hamming Distance = 1

---

## Q14 Can CRC Correct Errors?

No.

CRC only detects errors.

---

### Examiner Trap

Q. CRC detects or corrects?

Answer:

**Detects only.**

---

# Related Theory from Data Link Layer

## Functions of Data Link Layer

1. Framing
2. Error Control
3. Flow Control
4. Access Control

---

# Framing

Breaking data into frames.

---

# Error Control

Detecting transmission errors.

CRC belongs here.

---

# Flow Control

Controlling sender speed.

Methods:

* Stop and Wait
* Sliding Window

---

# Access Control

Determines who can transmit.

Examples:

* ALOHA
* CSMA/CD
* CSMA/CA

---

# Frequently Asked Numerical Viva

### Generator

```text
1011
```

How many zeros appended?

Length:

```text
4
```

Degree:

```text
3
```

Answer:

```text
000
```

---

### Generator

```text
10001
```

Length:

```text
5
```

Degree:

```text
4
```

Answer:

```text
0000
```

---

# One-Line Revision

| Question             | Answer                  |
| -------------------- | ----------------------- |
| CRC Full Form        | Cyclic Redundancy Check |
| Purpose              | Error Detection         |
| Layer                | Data Link Layer         |
| Arithmetic           | Modulo-2                |
| Operation            | XOR                     |
| Error Indication     | Non-zero remainder      |
| No Error             | Zero remainder          |
| CRC Correct Errors?  | No                      |
| Better Than Parity?  | Yes                     |
| Detect Burst Errors? | Yes                     |

---

# How to Score Full Marks in CRC Viva

If examiner asks:

**"Explain CRC."**

Say:

> "CRC is an error detection technique used at the Data Link Layer. The sender appends zeros equal to the degree of the generator polynomial and performs modulo-2 division using XOR operations. The remainder obtained is attached to the data and transmitted. The receiver performs the same division. If the remainder is zero, the frame is accepted; otherwise, an error is detected."

This answer alone usually covers 80% of CRC viva.

---

## Next Experiment (Very Important)

### Experiment 7: Framing Techniques

* Character Count
* Character Stuffing
* Bit Stuffing

This is another favorite programming + viva experiment from **Data Link Layer**, and examiners often ask it together with CRC.




# Experiment 7

# Framing Techniques in Data Link Layer

## Character Count, Character Stuffing and Bit Stuffing

🔥 **Very Important Practical + Viva Topic**

This experiment comes directly from **Data Link Layer** and is one of the examiner's favorite questions because it is easy to ask both theory and program logic.

---

# Aim

To study and implement different framing techniques:

1. Character Count
2. Character Stuffing
3. Bit Stuffing

used in the Data Link Layer.

---

# What is Framing?

When data is transmitted, it cannot be sent as one huge stream.

Data Link Layer divides data into smaller units called:

```text
Frames
```

This process is called:

```text
Framing
```

---

# Why Framing is Required?

Suppose sender sends:

```text
HELLOHOWAREYOU
```

Receiver must know:

* Where one frame starts
* Where one frame ends

Framing solves this problem.

---

# Data Link Layer Functions

1. Framing
2. Error Control
3. Flow Control
4. Access Control

Examiner often asks:

### Q. Which layer performs framing?

Answer:

**Data Link Layer**

---

# Framing Methods

There are three important framing techniques:

```text
1. Character Count
2. Character Stuffing
3. Bit Stuffing
```

---

# Method 1: Character Count

---

## Theory

The first field of every frame stores the total number of characters.

Example:

Data:

```text
HELLO
```

Length:

```text
5
```

Frame:

```text
5HELLO
```

---

## Example

Frame 1:

```text
5ABCDE
```

Frame 2:

```text
4WXYZ
```

---

## Working

Receiver reads first character.

If first character is:

```text
5
```

Receiver knows next 5 characters belong to frame.

---

## Advantage

Simple implementation.

---

## Disadvantage

Very Important Viva

Suppose count field becomes corrupted.

Example:

Original:

```text
5HELLO
```

Received:

```text
8HELLO
```

Receiver becomes confused.

Entire communication fails.

Therefore:

Character Count is rarely used today.

---

# Viva Questions

### Q. What is Character Count Method?

Length of frame stored at beginning.

---

### Q. Main disadvantage?

Count field corruption destroys synchronization.

---

### Q. Is Character Count widely used today?

No.

---

# Method 2: Character Stuffing

---

## Theory

Special characters are used to indicate:

* Start of frame
* End of frame

Example:

```text
DLE STX
```

Start

```text
DLE ETX
```

End

---

## Problem

Suppose actual data contains:

```text
DLE
```

Receiver may mistake it for control information.

---

# Solution

Character Stuffing

Extra escape character inserted.

---

## Example

Original Data

```text
HELLO DLE WORLD
```

After Stuffing

```text
HELLO DLE DLE WORLD
```

Extra DLE inserted.

---

## At Receiver

Extra DLE removed.

Original data recovered.

---

# Why Stuffing Needed?

To differentiate:

```text
Control Character
```

and

```text
Actual Data
```

---

# Viva Questions

### Q. What is Character Stuffing?

Insertion of extra escape characters into data.

---

### Q. Why Character Stuffing is used?

To prevent confusion between control characters and data.

---

### Q. Which protocol historically used Character Stuffing?

BISYNC

---

# Method 3: Bit Stuffing

⭐ MOST IMPORTANT

Examiners ask this very frequently.

---

# Theory

Frames are identified using a flag.

Common Flag:

```text
01111110
```

---

## Problem

Suppose data itself contains:

```text
01111110
```

Receiver may think frame ended.

---

# Solution

Bit Stuffing

Whenever:

```text
Five consecutive 1s
```

appear,

Sender inserts:

```text
0
```

---

# Rule

After:

```text
11111
```

Insert:

```text
0
```

---

# Example

Original Data

```text
1111101111110
```

---

## Stuffing

After every five 1s:

```text
1111100 11111010
```

Inserted zeros shown in bold conceptually.

---

# Receiver Side

Whenever receiver finds:

```text
111110
```

it removes inserted zero.

---

# Final Result

Original data restored.

---

# Why Bit Stuffing is Better?

Unlike Character Stuffing:

* Works with binary data
* Independent of character encoding
* Used in modern protocols

---

# Protocol Using Bit Stuffing

Very Important Viva

### HDLC

High-Level Data Link Control

Uses Bit Stuffing.

---

# Example Asked in Viva

Data:

```text
111111
```

Apply Bit Stuffing.

---

Five 1s occur:

```text
11111
```

Insert 0:

```text
1111101
```

Answer:

```text
1111101
```

---

# Another Example

Data:

```text
11111011111
```

Stuffed:

```text
1111100111110
```

---

# How to Explain Program

If examiner asks:

### Explain Bit Stuffing Program

Say:

> "In Bit Stuffing, whenever five consecutive 1s occur in the data, the sender inserts a 0 after them. At the receiver side this inserted 0 is removed. This prevents accidental occurrence of flag patterns inside the data."

---

# Comparison of Framing Techniques

| Method             | Technique              | Problem             |
| ------------------ | ---------------------- | ------------------- |
| Character Count    | Length field           | Count corruption    |
| Character Stuffing | Extra characters       | Character dependent |
| Bit Stuffing       | Insert 0 after five 1s | Best method         |

---

# Related Theory Questions

---

# What is HDLC?

Full Form:

```text
High-Level Data Link Control
```

Bit-oriented protocol.

Uses:

Bit Stuffing

---

### HDLC Flag

```text
01111110
```

Memorize this.

---

# What is a Frame?

Data unit of Data Link Layer.

---

# Difference Between Packet and Frame

| Packet        | Frame           |
| ------------- | --------------- |
| Network Layer | Data Link Layer |
| Uses IP       | Uses MAC        |

---

# Difference Between Frame and Segment

| Segment         | Frame           |
| --------------- | --------------- |
| Transport Layer | Data Link Layer |

---

# Common Examiner Questions

### Q1 What is framing?

Dividing data into frames.

---

### Q2 Which layer performs framing?

Data Link Layer.

---

### Q3 Why is framing needed?

To identify start and end of data.

---

### Q4 What is Character Count?

Frame length stored in beginning.

---

### Q5 Main disadvantage of Character Count?

Count field corruption.

---

### Q6 What is Character Stuffing?

Insertion of escape characters.

---

### Q7 Why Character Stuffing?

Avoid confusion between data and control characters.

---

### Q8 What is Bit Stuffing?

Insertion of 0 after five consecutive 1s.

---

### Q9 Why Bit Stuffing?

Prevent flag duplication inside data.

---

### Q10 Which protocol uses Bit Stuffing?

HDLC

---

### Q11 What is HDLC Flag?

```text
01111110
```

---

### Q12 What happens at receiver?

Stuffed bits are removed.

---

### Q13 Which framing technique is most commonly used?

Bit Stuffing.

---

### Q14 What is a Flag?

Special pattern marking frame boundaries.

---

### Q15 Why is Bit Stuffing better than Character Stuffing?

Works directly on binary data.

---

# Examiner's Rapid Fire Round

| Question                         | Answer                       |
| -------------------------------- | ---------------------------- |
| Framing Layer                    | Data Link Layer              |
| Data Link PDU                    | Frame                        |
| Network Layer PDU                | Packet                       |
| Transport Layer PDU              | Segment                      |
| HDLC Full Form                   | High-Level Data Link Control |
| HDLC Flag                        | 01111110                     |
| After how many 1s is 0 inserted? | 5                            |
| Character Count Problem          | Count corruption             |
| Character Stuffing Uses          | Escape characters            |
| Most Popular Method              | Bit Stuffing                 |

---

# Full Marks Viva Answer

If examiner asks:

### "Explain framing techniques."

Answer:

> "Framing is a Data Link Layer function used to divide a stream of bits into identifiable frames. The three main framing methods are Character Count, Character Stuffing and Bit Stuffing. Character Count stores frame length in the beginning, Character Stuffing inserts escape characters when control characters appear inside data, and Bit Stuffing inserts a 0 after every sequence of five consecutive 1s. Modern protocols such as HDLC use Bit Stuffing because it is efficient and independent of character encoding."

---

## Next Experiment (Very High Probability)

### Experiment 8: Routing Algorithms – Dijkstra's Shortest Path Algorithm

This belongs to **Network Layer** and **OSPF Routing**, and examiners frequently ask:

* Dijkstra Algorithm
* OSPF
* RIP vs OSPF
* Distance Vector vs Link State
* Routing Tables
* Shortest Path Calculation

It is one of the most common programming practicals after CRC and Framing.





# Experiment 8

# Dijkstra's Shortest Path Algorithm (Routing Algorithm)

🔥 **One of the most important CN programming practicals.**

This experiment belongs to:

* Network Layer
* Routing
* OSPF Protocol
* Link State Routing

Examiners love this experiment because they can ask both:

* Programming logic
* Routing theory

---

# Aim

To implement Dijkstra's Algorithm for finding the shortest path between source and destination nodes in a network.

---

# Why Routing is Needed?

Consider this network:

```text
A ---- B ---- D
|      |
|      |
C ---- E
```

If A wants to send data to D,

multiple paths may exist.

Routing determines:

> Which path is the shortest and most efficient?

---

# What is Routing?

Routing is the process of selecting the best path for packet transmission.

Performed at:

### Network Layer (Layer 3)

---

# What is a Router?

A router:

* Connects different networks
* Uses routing tables
* Forwards packets based on IP address

---

# Types of Routing

## 1. Static Routing

Configured manually.

Advantages:

* Simple

Disadvantages:

* Difficult in large networks

---

## 2. Dynamic Routing

Routes calculated automatically.

Examples:

* RIP
* OSPF
* EIGRP
* BGP

---

# What is Dijkstra's Algorithm?

Dijkstra's Algorithm finds:

### Shortest Path

from a source node to all other nodes.

Used by:

### OSPF (Open Shortest Path First)

---

# Very Important Viva

### Q. Which routing protocol uses Dijkstra?

Answer:

**OSPF**

---

# Example Network

Consider:

```text
      2
   A ----- B
   |       |
  5|       |3
   |       |
   C ----- D
       1
```

---

# Goal

Find shortest path from:

```text
A
```

to

```text
D
```

---

# Step 1

Initialize:

| Node | Distance |
| ---- | -------- |
| A    | 0        |
| B    | ∞        |
| C    | ∞        |
| D    | ∞        |

---

# Step 2

Choose smallest node.

Current:

```text
A
```

Update neighbors.

---

# Distances

```text
A → B = 2
A → C = 5
```

Table:

| Node | Distance |
| ---- | -------- |
| A    | 0        |
| B    | 2        |
| C    | 5        |
| D    | ∞        |

---

# Step 3

Select smallest unvisited node.

```text
B
```

Distance:

```text
2
```

---

Update:

```text
B → D = 3
```

New distance:

```text
2 + 3 = 5
```

---

Table:

| Node | Distance |
| ---- | -------- |
| A    | 0        |
| B    | 2        |
| C    | 5        |
| D    | 5        |

---

# Step 4

Visit D.

Algorithm ends.

---

# Result

Shortest path:

```text
A → B → D
```

Cost:

```text
5
```

---

# Dijkstra Algorithm Steps

1. Set source distance = 0.
2. Set all others = ∞.
3. Choose smallest unvisited node.
4. Update neighbor distances.
5. Mark node visited.
6. Repeat until all nodes visited.

---

# How to Explain Program

If examiner asks:

### Explain your Dijkstra program.

Say:

> "The program finds the shortest path between nodes using Dijkstra's Algorithm. Initially the source node distance is set to zero and all others are set to infinity. The node with minimum distance is selected repeatedly and neighbor distances are updated. Finally the shortest path and minimum cost are obtained."

---

# What is Cost?

Cost represents:

* Distance
* Delay
* Bandwidth metric

depending on routing protocol.

---

# Why Dijkstra Works?

Because it always expands the nearest node first.

This ensures optimal shortest paths.

---

# Time Complexity

Most viva answer:

```text
O(V²)
```

Where:

V = Number of vertices

---

# OSPF (Very Important)

---

## Full Form

Open Shortest Path First

---

## Type

Link State Routing Protocol

---

## Uses

Dijkstra Algorithm

---

## Advantages

* Fast convergence
* Efficient routing
* Scalable

---

# OSPF Working

Each router:

1. Learns topology
2. Builds database
3. Runs Dijkstra
4. Creates routing table

---

# Link State Routing

Each router knows:

Entire network topology.

Example:

```text
Router A
knows all routers and links.
```

---

# Distance Vector Routing

Each router knows:

Only neighboring routes.

Example:

```text
Router A
knows next hop only.
```

---

# Distance Vector vs Link State

| Distance Vector | Link State    |
| --------------- | ------------- |
| RIP             | OSPF          |
| Slow            | Fast          |
| Hop Count       | Cost          |
| Less accurate   | More accurate |

---

# RIP

## Full Form

Routing Information Protocol

---

# Metric Used

Hop Count

---

# Maximum Hops

```text
15
```

Very important viva.

---

# OSPF Metric

Uses:

```text
Cost
```

instead of hop count.

---

# RIP vs OSPF

| RIP             | OSPF           |
| --------------- | -------------- |
| Distance Vector | Link State     |
| Hop Count       | Cost           |
| Slow            | Fast           |
| Max 15 Hops     | No such limit  |
| Small Networks  | Large Networks |

---

# Routing Table

Stores:

| Destination | Next Hop |
| ----------- | -------- |
| Network A   | Router 1 |
| Network B   | Router 2 |

---

# Packet Forwarding

Router checks:

1. Destination IP
2. Routing Table
3. Next Hop

Then forwards packet.

---

# Related Theory from Network Layer

---

# Functions of Network Layer

1. Routing
2. Logical Addressing
3. Packet Forwarding
4. Congestion Control

---

# IP Address

Logical address.

Example:

```text
192.168.1.10
```

---

# IPv4

Length:

```text
32 bits
```

---

# IPv6

Length:

```text
128 bits
```

---

# Default Gateway

Router used to reach other networks.

---

# NAT

Network Address Translation

Converts:

```text
Private IP → Public IP
```

---

# Frequently Asked Viva Questions

## Q1 What is Routing?

Finding best path for packets.

---

## Q2 Which layer performs routing?

Network Layer.

---

## Q3 What is Dijkstra Algorithm?

Shortest path algorithm.

---

## Q4 Which routing protocol uses Dijkstra?

OSPF.

---

## Q5 Full Form of OSPF?

Open Shortest Path First.

---

## Q6 What type of routing protocol is OSPF?

Link State Routing Protocol.

---

## Q7 What is a Router?

Device that forwards packets between networks.

---

## Q8 Which address does Router use?

IP Address.

---

## Q9 What is Routing Table?

Table storing route information.

---

## Q10 What is Hop Count?

Number of routers crossed.

---

## Q11 Which protocol uses Hop Count?

RIP.

---

## Q12 Maximum Hop Count in RIP?

```text
15
```

---

## Q13 What metric does OSPF use?

Cost.

---

## Q14 Which is better, RIP or OSPF?

OSPF.

---

## Q15 Why?

Faster convergence and better routing decisions.

---

# Examiner's Numerical Questions

### Network

```text
A ----2---- B
|           |
5           3
|           |
C ----1---- D
```

Find shortest path A → D.

Answer:

```text
A → B → D
```

Cost:

```text
5
```

---

### Why not A → C → D?

Cost:

```text
5 + 1 = 6
```

Higher.

---

# Common Trap Questions

### Q. Does Dijkstra work with negative weights?

Answer:

No.

---

### Q. Does OSPF use Hop Count?

Answer:

No.

Uses Cost.

---

### Q. Which is Link State Protocol?

Answer:

OSPF.

---

### Q. Which is Distance Vector Protocol?

Answer:

RIP.

---

# Quick Revision Table

| Question             | Answer                   |
| -------------------- | ------------------------ |
| Routing Layer        | Network Layer            |
| Dijkstra Purpose     | Shortest Path            |
| OSPF Full Form       | Open Shortest Path First |
| OSPF Type            | Link State               |
| RIP Type             | Distance Vector          |
| RIP Metric           | Hop Count                |
| RIP Max Hops         | 15                       |
| OSPF Metric          | Cost                     |
| Router Uses          | IP Address               |
| Routing Table Stores | Routes                   |

---

# Full Marks Viva Answer

If examiner asks:

### "Explain Dijkstra Algorithm."

Answer:

> "Dijkstra's Algorithm is a shortest path routing algorithm used in OSPF. It starts from a source node with distance zero and repeatedly selects the nearest unvisited node. Neighbor distances are updated until all nodes are processed. The final result provides the shortest path and minimum cost route to every destination."

---

## Next Experiment

### Experiment 9: IP Addressing and Classification (Class A, B, C, D, E)

This is another extremely common programming practical where you are given an IP address and must determine:

* Class
* Network ID
* Host ID
* Default Mask
* Number of Hosts

It generates a huge number of viva questions from **Network Layer and IPv4 Addressing**.



# Experiment 9

# IP Addressing and IP Address Classification (Class A, B, C, D, E)

🔥 **This is one of the most frequently asked CN practicals.**

Many colleges give a program like:

> "Enter an IP Address and determine its class."

Then the viva expands into:

* IPv4
* IPv6
* Subnet Mask
* Network ID
* Host ID
* Public/Private IP
* DHCP
* NAT

---

# Aim

To identify:

* Class of IP Address
* Network ID
* Host ID
* Default Subnet Mask

for a given IPv4 address.

---

# What is an IP Address?

IP = Internet Protocol Address

It is a **logical address** used to uniquely identify a device on a network.

Example:

```text
192.168.1.10
```

---

# Why IP Address is Required?

Imagine sending a letter.

You need:

* House Number
* Street
* City

Similarly, packets need:

```text
Destination IP Address
```

to reach the correct device.

---

# IPv4 Address

Length:

```text
32 bits
```

Divided into:

```text
4 Octets
```

Example:

```text
192.168.1.10
```

---

# Binary Representation

```text
192 = 11000000
168 = 10101000
1   = 00000001
10  = 00001010
```

Total:

```text
32 bits
```

---

# IPv6 Address

Introduced because IPv4 addresses were running out.

Length:

```text
128 bits
```

Example:

```text
2001:db8::1
```

---

# IPv4 Address Structure

IP Address consists of:

```text
Network ID + Host ID
```

Example:

```text
192.168.1.10
```

Network identifies network.

Host identifies device.

---

# Classful Addressing

IPv4 is divided into five classes.

---

# Class A

Range:

```text
1 – 126
```

First Octet determines class.

Example:

```text
10.1.2.3
```

---

## Default Mask

```text
255.0.0.0
```

---

## Network Portion

```text
First Octet
```

---

## Host Portion

```text
Remaining Three Octets
```

---

# Class B

Range:

```text
128 – 191
```

Example:

```text
172.16.1.5
```

---

## Default Mask

```text
255.255.0.0
```

---

## Network Portion

First 2 octets

---

## Host Portion

Last 2 octets

---

# Class C

Range:

```text
192 – 223
```

Example:

```text
192.168.1.10
```

---

## Default Mask

```text
255.255.255.0
```

---

## Network Portion

First 3 octets

---

## Host Portion

Last octet

---

# Class D

Range:

```text
224 – 239
```

Purpose:

```text
Multicasting
```

---

# Class E

Range:

```text
240 – 255
```

Purpose:

```text
Experimental
```

---

# Quick Class Identification Trick

Look only at first octet.

| First Octet | Class |
| ----------- | ----- |
| 1-126       | A     |
| 128-191     | B     |
| 192-223     | C     |
| 224-239     | D     |
| 240-255     | E     |

---

# Examples

### Example 1

IP:

```text
10.20.30.40
```

First octet:

```text
10
```

Class:

```text
A
```

---

### Example 2

IP:

```text
172.16.10.5
```

First octet:

```text
172
```

Class:

```text
B
```

---

### Example 3

IP:

```text
192.168.1.10
```

First octet:

```text
192
```

Class:

```text
C
```

---

# Network ID and Host ID

Examiner asks this very often.

---

## Example

IP:

```text
192.168.1.10
```

Class:

```text
C
```

Default Mask:

```text
255.255.255.0
```

Network ID:

```text
192.168.1
```

Host ID:

```text
10
```

---

## Example

IP:

```text
172.16.20.100
```

Class:

```text
B
```

Network ID:

```text
172.16
```

Host ID:

```text
20.100
```

---

# Private IP Addresses

Very Important Viva.

---

## Class A Private

```text
10.0.0.0 – 10.255.255.255
```

---

## Class B Private

```text
172.16.0.0 – 172.31.255.255
```

---

## Class C Private

```text
192.168.0.0 – 192.168.255.255
```

---

# Public IP Address

Used on Internet.

Assigned by ISP.

Example:

```text
8.8.8.8
```

---

# NAT

Network Address Translation

Converts:

```text
Private IP → Public IP
```

Used by routers.

---

# Loopback Address

Very common viva.

```text
127.0.0.1
```

Represents:

```text
Local Machine
```

---

# Why Use Loopback?

Testing TCP/IP stack.

Command:

```cmd
ping 127.0.0.1
```

---

# Special Addresses

### Network Address

All host bits = 0

Example:

```text
192.168.1.0
```

---

### Broadcast Address

All host bits = 1

Example:

```text
192.168.1.255
```

---

# Subnet Mask

Determines:

```text
Network Portion
Host Portion
```

---

# Default Masks

| Class | Mask          |
| ----- | ------------- |
| A     | 255.0.0.0     |
| B     | 255.255.0.0   |
| C     | 255.255.255.0 |

---

# Number of Hosts

Examiner may ask.

Formula:

2^h-2

where:

```text
h = Host bits
```

---

## Class C

Host Bits:

```text
8
```

Hosts:

```text
2⁸ - 2 = 254
```

---

## Class B

Host Bits:

```text
16
```

Hosts:

```text
65534
```

---

## Class A

Host Bits:

```text
24
```

Hosts:

```text
16777214
```

---

# How to Explain Program

> "The program accepts an IPv4 address and determines its class based on the first octet. According to the class, the default subnet mask, network ID and host ID are identified. This helps understand logical addressing in computer networks."

---

# Important Viva Questions

## Q1 What is IP Address?

Logical address of a device.

---

## Q2 Which layer uses IP Address?

Network Layer.

---

## Q3 IPv4 length?

```text
32 bits
```

---

## Q4 IPv6 length?

```text
128 bits
```

---

## Q5 Which class does 192.168.1.1 belong to?

Class C.

---

## Q6 Which class does 172.16.1.1 belong to?

Class B.

---

## Q7 Which class does 10.1.1.1 belong to?

Class A.

---

## Q8 What is subnet mask?

Separates network and host portions.

---

## Q9 What is Network ID?

Identifies network.

---

## Q10 What is Host ID?

Identifies host inside network.

---

## Q11 What is Loopback Address?

```text
127.0.0.1
```

---

## Q12 What is NAT?

Network Address Translation.

---

## Q13 Why NAT is used?

To conserve public IP addresses.

---

## Q14 Difference Between MAC and IP?

| MAC              | IP              |
| ---------------- | --------------- |
| Physical Address | Logical Address |
| Layer 2          | Layer 3         |
| Permanent        | Can change      |

---

## Q15 What is Broadcast Address?

Address used to send data to all hosts.

---

# Examiner's Favorite Numerical Questions

### IP:

```text
192.168.1.10
```

Class?

Answer:

```text
Class C
```

Network ID?

```text
192.168.1
```

Host ID?

```text
10
```

Mask?

```text
255.255.255.0
```

---

### IP:

```text
172.20.10.5
```

Class?

```text
Class B
```

Network ID?

```text
172.20
```

Host ID?

```text
10.5
```

Mask?

```text
255.255.0.0
```

---

# Rapid-Fire Viva

| Question         | Answer                      |
| ---------------- | --------------------------- |
| IPv4 Length      | 32 bits                     |
| IPv6 Length      | 128 bits                    |
| Loopback Address | 127.0.0.1                   |
| Class A Range    | 1-126                       |
| Class B Range    | 128-191                     |
| Class C Range    | 192-223                     |
| Class D Purpose  | Multicast                   |
| Class E Purpose  | Experimental                |
| NAT Full Form    | Network Address Translation |
| Layer Using IP   | Network Layer               |

---

# Full Marks Viva Answer

If examiner asks:

### "Explain IP Addressing."

Answer:

> "IP addressing is a logical addressing scheme used at the Network Layer. IPv4 addresses are 32 bits long and are divided into network and host portions. Based on the first octet, addresses are classified into Classes A, B, C, D and E. Routers use IP addresses to forward packets between networks."

---

## Next Experiment (Usually the Last Major CN Practical)

### Experiment 10: Packet Tracer – Design and Simulation of Networks

This is often considered the most important practical because examiners ask about:

* Routers
* Switches
* VLANs
* Routing
* DHCP
* DNS
* LAN/WAN
* OSI Model
* Packet Flow

and it can pull viva questions from **the entire syllabus**.




# Experiment 10

# Cisco Packet Tracer – Design and Simulation of Computer Networks

🔥 **This is usually the final and highest-weightage CN practical.**

Why?

Because Packet Tracer combines:

* OSI Model
* IP Addressing
* Routing
* Switching
* DHCP
* DNS
* LAN
* WAN
* Network Devices

A viva from Packet Tracer can cover the **entire syllabus**.

---

# Aim

To design, configure, and simulate a computer network using Cisco Packet Tracer.

---

# What is Cisco Packet Tracer?

Cisco Packet Tracer is a network simulation software developed by Cisco.

Used for:

* Designing networks
* Configuring routers
* Configuring switches
* Testing connectivity
* Learning networking concepts

---

# Why Use Packet Tracer?

Building a real network is expensive.

Packet Tracer allows simulation without actual hardware.

---

# Important Viva

### Q. What is Packet Tracer?

A network simulation and learning tool developed by Cisco.

---

### Q. Why use Packet Tracer?

To design and test networks virtually.

---

# Common Devices Used

---

## PC

End device.

Used by users.

---

## Switch

Layer:

```text
Layer 2
```

Uses:

```text
MAC Address
```

---

## Router

Layer:

```text
Layer 3
```

Uses:

```text
IP Address
```

---

## Hub

Layer:

```text
Layer 1
```

Broadcasts everything.

---

## Server

Provides services such as:

* DHCP
* DNS
* Web
* FTP

---

# Simple LAN Topology

```text
PC1 -----\
          \
           Switch
          /
PC2 -----/
```

---

# Procedure

## Step 1

Open Packet Tracer.

---

## Step 2

Drag devices:

* 2 PCs
* 1 Switch

---

## Step 3

Connect using:

```text
Copper Straight Through Cable
```

---

## Step 4

Assign IP Addresses.

PC1:

```text
192.168.1.10
```

PC2:

```text
192.168.1.20
```

Mask:

```text
255.255.255.0
```

---

## Step 5

Verify connectivity.

Command Prompt:

```bash
ping 192.168.1.20
```

---

## Output

```text
Reply from 192.168.1.20
```

Network working successfully.

---

# How Packet Travels

Examiner's favorite question.

Suppose:

```text
PC1 → PC2
```

---

### Step 1

Application creates data.

---

### Step 2

Transport Layer adds TCP header.

---

### Step 3

Network Layer adds IP header.

---

### Step 4

Data Link Layer adds MAC header.

---

### Step 5

Frame sent to switch.

---

### Step 6

Switch checks MAC table.

---

### Step 7

Switch forwards frame.

---

### Step 8

PC2 receives frame.

---

# Simulation Mode

Packet Tracer has:

## Real-Time Mode

Network operates normally.

---

## Simulation Mode

Shows packet movement step-by-step.

Very useful for viva.

---

# Switch Configuration

---

## MAC Address Table

Switch learns:

```text
MAC Address → Port
```

Example:

| MAC   | Port  |
| ----- | ----- |
| AA-AA | Fa0/1 |
| BB-BB | Fa0/2 |

---

# Important Viva

### Q. How does switch learn addresses?

By observing source MAC addresses.

---

### Q. What happens if destination MAC unknown?

Switch floods frame.

---

# Router Configuration

Example:

```text
PC1 --- Router --- PC2
```

---

Router Interfaces:

```text
Fa0/0
Fa0/1
```

Need IP assignment.

---

Example:

Interface 1:

```text
192.168.1.1
```

Interface 2:

```text
192.168.2.1
```

---

# Routing

Router forwards packets between networks.

---

# Static Routing

Routes manually configured.

Example:

```text
ip route
```

command.

---

# Dynamic Routing

Routes learned automatically.

Examples:

* RIP
* OSPF
* EIGRP

---

# RIP

Routing Information Protocol

Metric:

```text
Hop Count
```

Maximum:

```text
15 hops
```

---

# OSPF

Open Shortest Path First

Uses:

Dijkstra Algorithm

Metric:

```text
Cost
```

---

# DHCP Configuration

Very frequently asked.

---

# What is DHCP?

Dynamic Host Configuration Protocol

Automatically assigns:

* IP Address
* Subnet Mask
* Gateway
* DNS

---

# DHCP Process

Remember:

```text
DORA
```

---

## D

Discover

---

## O

Offer

---

## R

Request

---

## A

Acknowledge

---

# DHCP Ports

Server:

```text
67
```

Client:

```text
68
```

---

# DNS Configuration

---

## DNS

Domain Name System

Converts:

```text
google.com
```

↓

```text
142.x.x.x
```

---

# DNS Port

```text
53
```

---

# Web Server

Used to host websites.

Protocols:

* HTTP
* HTTPS

---

# HTTP

Port:

```text
80
```

---

# HTTPS

Port:

```text
443
```

---

# FTP Server

Used for file transfer.

Port:

```text
21
```

---

# Telnet

Port:

```text
23
```

Used for remote access.

(Insecure)

---

# SSH

Port:

```text
22
```

Secure remote access.

---

# VLAN (Very Common Viva)

---

## VLAN

Virtual Local Area Network

Used to divide one switch into multiple logical networks.

---

Example

Switch:

```text
VLAN 10 → Sales
VLAN 20 → HR
```

---

# Advantage

Improves:

* Security
* Traffic management

---

# VLAN Communication

Different VLANs require:

```text
Router
```

or

```text
Layer 3 Switch
```

---

# Network Troubleshooting

Commands used:

```bash
ipconfig
ping
tracert
arp -a
nslookup
netstat
```

---

# Important Viva Questions

## Q1 What is Packet Tracer?

Cisco network simulation software.

---

## Q2 Who developed Packet Tracer?

Cisco.

---

## Q3 Difference between Simulation and Real-Time mode?

Simulation shows packet flow.

Real-Time operates normally.

---

## Q4 Which cable connects PC to Switch?

Straight-through cable.

---

## Q5 Which cable connects PC to PC?

Cross-over cable.

---

## Q6 Which layer does Switch work on?

Layer 2.

---

## Q7 Which layer does Router work on?

Layer 3.

---

## Q8 Which address does Switch use?

MAC Address.

---

## Q9 Which address does Router use?

IP Address.

---

## Q10 What is DHCP?

Automatic IP allocation protocol.

---

## Q11 DHCP Process?

DORA.

---

## Q12 What is DNS?

Domain Name System.

---

## Q13 DNS Port?

53.

---

## Q14 What is VLAN?

Virtual Local Area Network.

---

## Q15 Why VLAN?

Improves security and management.

---

## Q16 What is Routing?

Finding best path for packets.

---

## Q17 Which protocol uses Dijkstra?

OSPF.

---

## Q18 Which protocol uses Hop Count?

RIP.

---

## Q19 Maximum RIP Hops?

15.

---

## Q20 What is Default Gateway?

Router address used to reach other networks.

---

# Most Common Examiner Scenario Questions

### Scenario 1

PC1 cannot ping PC2.

Possible reasons:

* Wrong IP
* Wrong subnet mask
* Cable disconnected
* Switch issue

---

### Scenario 2

PC can ping gateway but not internet.

Possible reasons:

* DNS issue
* ISP issue
* Routing issue

---

### Scenario 3

DHCP not assigning IP.

Possible reasons:

* DHCP service down
* Wrong pool configuration
* Physical connectivity issue

---

# Complete Port Number Cheat Sheet

| Protocol    | Port |
| ----------- | ---- |
| FTP         | 21   |
| SSH         | 22   |
| Telnet      | 23   |
| SMTP        | 25   |
| DNS         | 53   |
| DHCP Server | 67   |
| DHCP Client | 68   |
| HTTP        | 80   |
| HTTPS       | 443  |

⚠️ These are among the most asked viva questions.

---

# 25 Questions Examiners Ask Repeatedly

1. What is OSI Model?
2. How many layers in OSI?
3. Difference between Hub and Switch?
4. Difference between Switch and Router?
5. What is MAC Address?
6. What is IP Address?
7. Difference between MAC and IP?
8. What is ARP?
9. What is DHCP?
10. What is DNS?
11. What is NAT?
12. What is Ping?
13. What is ICMP?
14. What is TCP?
15. What is UDP?
16. Difference between TCP and UDP?
17. What is CRC?
18. What is Framing?
19. What is Bit Stuffing?
20. What is Dijkstra Algorithm?
21. What is OSPF?
22. What is RIP?
23. What is VLAN?
24. What is Packet Tracer?
25. What is Default Gateway?

---

# Final 5-Minute Revision Before Entering the Lab

### Layers

OSI = 7 Layers

### Addresses

* MAC = 48 bits
* IPv4 = 32 bits
* IPv6 = 128 bits

### Devices

* Hub = Layer 1
* Switch = Layer 2
* Router = Layer 3

### Protocols

* ARP = IP → MAC
* DNS = Name → IP
* DHCP = Automatic IP
* ICMP = Ping

### Routing

* RIP = Hop Count
* OSPF = Dijkstra + Cost

### Framing

* Character Count
* Character Stuffing
* Bit Stuffing

### Error Detection

* Parity
* Checksum
* CRC

### TCP Handshake

```text
SYN → SYN-ACK → ACK
```

### Ports

* FTP = 21
* SSH = 22
* Telnet = 23
* DNS = 53
* HTTP = 80
* HTTPS = 443

If you can answer these confidently, you'll handle about **90–95% of typical CN practical viva questions**.



