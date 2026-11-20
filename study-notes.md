# Introduction to Computer Networks — Study Notes

These notes provide a concise introduction to the topics covered in the accompanying teaching material. They are intended to support classroom learning and revision.

## 1. Data communication

Data communication is the exchange of data between devices through a transmission medium. The medium may be wired, such as a cable, or wireless.

When studying a data communication system, identify:
- the devices that communicate;
- the data being exchanged;
- the transmission medium carrying the signal.

## 2. Computer networks

A computer network is a collection of devices connected through communication links. A connected device is commonly called a **node**. Examples include computers and printers. A **link** is the medium that carries information between nodes; it may use cable, air, or optical fibre.

## 3. Classification of networks

### By geographical coverage

- **LAN (Local Area Network):** covers a limited local area.
- **MAN (Metropolitan Area Network):** spans a metropolitan or city-scale area.
- **WAN (Wide Area Network):** spans a large geographical area.

### By component roles

- **Peer-to-peer:** connected computers can share resources directly; there are no permanently assigned client and server roles in the basic model.
- **Client-server:** clients request services or resources from a server.

### By connection type

- **Point-to-point:** a dedicated link connects two devices.
- **Multipoint:** more than two devices share a link.

## 4. Network topology

A physical network topology describes how network devices and links are arranged.

### Bus
A single main cable connects the nodes. Terminators are used at the ends to prevent signal reflections. The arrangement can be inexpensive, but it can be difficult to troubleshoot and is not highly scalable.

### Star
Each node connects to a central device, such as a hub or switch. It is relatively easy to manage and expand. The central device is a critical dependency: if it fails, connected communication may be disrupted.

### Ring
Devices are connected in a continuous loop. A failure in a node or link can disrupt a basic single-ring network. A dual-ring design is one approach used to improve resilience.

### Mesh
Devices are connected through multiple links. A fully connected mesh provides a direct link between every pair of devices, but requires many connections.

### Tree or hybrid
A tree or hybrid design combines features of other topologies. For example, groups of star-connected devices may connect to a shared backbone.

## 5. Transmission media

Transmission media carry signals between network devices.

### Guided media

- **Twisted-pair cable:** pairs of insulated wires are twisted together. It is commonly used in telephone systems, buildings, and LANs. It is relatively inexpensive and easy to work with, but has distance, bandwidth, and interference limitations. Near-end crosstalk occurs when a signal from one pair couples into another pair near the transmitting end.
- **Unshielded twisted pair (UTP):** does not have the additional metallic shielding found in STP and is generally easier and less expensive to install.
- **Shielded twisted pair (STP):** includes shielding to reduce electromagnetic interference; it is typically thicker, heavier, and more expensive.
- **Coaxial cable:** used in applications such as television distribution, cable TV, and some data links.
- **Optical fibre:** carries information using light. Its benefits include high capacity, low attenuation, low weight, and immunity to electromagnetic interference.

### Wireless transmission

Wireless communication uses electromagnetic waves. Examples discussed in the teaching material include:
- **Radio waves:** used for multicast applications such as radio and television broadcasting.
- **Microwaves:** used for unicast applications such as cellular, satellite, and wireless LAN communication.
- **Infrared:** suitable for short-range communication in a closed area, typically requiring line of sight.

## 6. Connecting devices

- **Hub:** connects devices and repeats incoming data to its other ports. It does not make forwarding decisions based on the destination.
- **Switch:** connects devices in a network and uses MAC addresses to forward frames toward the intended device.
- **Router:** connects different networks and uses IP addressing and routing information to forward packets.

## 7. Protocols

A network protocol is a set of rules governing communication. It specifies what is communicated, how it is communicated, and when it is communicated.

The key elements are:
- **Syntax:** the structure or format of the data.
- **Semantics:** the meaning of the fields and what action they indicate.
- **Timing:** when data should be sent and at what rate.

## 8. OSI reference model

The OSI (Open Systems Interconnection) model is a reference model for understanding and designing network communication. It is a model, not a network protocol.

The seven layers, from bottom to top, are:

1. **Physical:** transmits individual bits over a physical medium; concerns interfaces, signals, data rate, physical topology, and transmission mode.
2. **Data Link:** provides node-to-node delivery using frames; includes framing, physical addressing, flow control, error control, and access control.
3. **Network:** supports source-to-destination packet delivery across interconnected networks; includes logical addressing and routing.
4. **Transport:** provides process-to-process delivery; includes port addressing, segmentation and reassembly, connection control, flow control, and error control.
5. **Session:** establishes, maintains, and synchronises interactions between communicating systems.
6. **Presentation:** handles the representation of exchanged information, including translation, encryption/decryption, and compression.
7. **Application:** provides network services to user applications, such as electronic mail and remote file access.

## 9. TCP/IP reference model

The teaching presentation also introduces the TCP/IP reference model and compares it with the OSI model. Use the model diagram discussed in class to identify its layers and relate their responsibilities to the OSI layers.

## Quick comparison: hub, switch, and router

| Device | Main role | Addressing / forwarding idea |
|---|---|---|
| Hub | Connects devices and repeats received signals to other ports | Does not selectively forward based on destination |
| Switch | Connects devices within a network | Uses MAC addresses to forward frames |
| Router | Connects different networks | Uses IP addresses and routing decisions to forward packets |

## Revision checklist

- [ ] I can define data communication, node, link, and network.
- [ ] I can distinguish LAN, MAN, and WAN.
- [ ] I can explain peer-to-peer and client-server networks.
- [ ] I can draw and compare bus, star, ring, mesh, and hybrid topologies.
- [ ] I can distinguish twisted pair, coaxial cable, optical fibre, and wireless media.
- [ ] I can explain the roles of a hub, switch, and router.
- [ ] I can define protocol, syntax, semantics, and timing.
- [ ] I can name the seven OSI layers in order and explain their main functions.
- [ ] I can explain why the OSI model is a reference model rather than a protocol.
