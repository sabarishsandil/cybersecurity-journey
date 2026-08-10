# Day 2 - Networking

# OSI Model

## 1. What is the OSI Model?

OSI stands for:

Open Systems Interconnection

The OSI model is a conceptual model used to understand how devices communicate over a network.

It divides network communication into 7 layers.

The 7 layers are:

7 - Application
6 - Presentation
5 - Session
4 - Transport
3 - Network
2 - Data Link
1 - Physical

Each layer performs a different function.

---

# 2. Layer 7 - Application

The Application layer is the closest layer to the user and applications.

It provides network services used by applications.

Examples of protocols:

- HTTP
- HTTPS
- DNS
- SSH
- FTP
- SMTP

Examples:

Web browser → HTTP/HTTPS
DNS lookup → DNS
Remote login → SSH
Email → SMTP

Important:

The Application layer does not mean the actual application such as Chrome or Firefox. It refers to the network protocols and services used by applications.

---

# 3. Layer 6 - Presentation

The Presentation layer deals with how data is represented.

Main responsibilities include:

- Data formatting
- Data encoding
- Encryption
- Decryption
- Compression
- Decompression

The purpose is to make sure that data sent by one system can be understood by another system.

Examples:

- Encryption
- Character encoding
- Data compression

---

# 4. Layer 5 - Session

The Session layer manages communication sessions between applications.

It can be thought of as managing:

Start session
↓
Maintain session
↓
End session

Its responsibilities can include:

- Establishing sessions
- Maintaining sessions
- Terminating sessions
- Managing communication between applications

---

# 5. Layer 4 - Transport

The Transport layer provides end-to-end communication between devices and applications.

The two major protocols are:

- TCP
- UDP

## TCP

TCP stands for Transmission Control Protocol.

TCP provides:

- Reliable delivery
- Ordered delivery
- Error checking
- Connection-oriented communication

TCP is commonly used when reliable delivery is important.

Examples:

- HTTPS
- SSH
- FTP

## UDP

UDP stands for User Datagram Protocol.

UDP is:

- Connectionless
- Lightweight
- Faster in many situations
- Does not guarantee delivery or ordering

Examples:

- DNS
- Streaming
- Online gaming
- Voice/video communication

---

# 6. Layer 3 - Network

The Network layer is responsible for logical addressing and routing.

The main concept is:

IP Address

Example:

192.168.1.10

Routers operate primarily at this layer.

Important functions:

- Logical addressing
- Routing
- Packet forwarding

Important protocol:

- IP

Example:

Computer A
     |
     | IP Packet
     ↓
   Router
     |
     ↓
Computer B

The router uses destination IP information to help forward the packet toward its destination.

---

# 7. Layer 2 - Data Link

The Data Link layer is responsible for communication between devices on the same local network.

Important concept:

MAC Address

A MAC address identifies a network interface.

Examples of technologies associated with this layer:

- Ethernet
- Wi-Fi

The Data Link layer deals with frames.

Important concepts:

- MAC addresses
- Frames
- Switches
- Local network communication

---

# 8. Layer 1 - Physical

The Physical layer is the lowest layer of the OSI model.

It deals with the physical transmission of bits.

Examples:

- Ethernet cables
- Fiber-optic cables
- Radio signals
- Electrical signals
- Network connectors

Data at this layer is represented as bits:

0 and 1

---

# 9. OSI Model Summary

| Layer | Name | Main Function | Examples |
|------|------|---------------|----------|
| 7 | Application | Network services for applications | HTTP, HTTPS, DNS, SSH |
| 6 | Presentation | Data representation and encryption | Encoding, encryption |
| 5 | Session | Manage communication sessions | Session management |
| 4 | Transport | End-to-end communication | TCP, UDP |
| 3 | Network | Routing and logical addressing | IP, Routers |
| 2 | Data Link | Local network communication | MAC, Ethernet, Wi-Fi |
| 1 | Physical | Transmission of bits | Cables, radio, fiber |

---

# 10. OSI Data Flow

When data is sent from one computer to another, it passes through the layers.

Example:

Application
     ↓
Presentation
     ↓
Session
     ↓
Transport
     ↓
Network
     ↓
Data Link
     ↓
Physical

At the receiving computer, the process happens in the opposite direction.

Physical
     ↓
Data Link
     ↓
Network
     ↓
Transport
     ↓
Session
     ↓
Presentation
     ↓
Application

---

# 11. Data Units

Different OSI layers commonly use different names for data.

Layer 7-5:

Data

Layer 4:

TCP → Segment
UDP → Datagram

Layer 3:

Packet

Layer 2:

Frame

Layer 1:

Bits

Simplified:

Data
 ↓
Segment / Datagram
 ↓
Packet
 ↓
Frame
 ↓
Bits

---

# 12. OSI Layer Examples

## When opening a website

Suppose I open:

https://example.com

The communication can be understood using the OSI layers.

Layer 7 - Application

HTTPS is used by the application.

Layer 6 - Presentation

Data representation and encryption are relevant here.

Layer 5 - Session

The communication session is managed.

Layer 4 - Transport

TCP provides transport communication.

Layer 3 - Network

IP handles addressing and routing.

Layer 2 - Data Link

Ethernet or Wi-Fi handles local network communication.

Layer 1 - Physical

Bits travel through a cable or wireless signal.

---

# 13. OSI and Cybersecurity

Understanding the OSI model is important in cybersecurity because different attacks and security controls can occur at different layers.

Examples:

Layer 1 - Physical

- Cable attacks
- Physical device access

Layer 2 - Data Link

- MAC spoofing
- ARP-related attacks

Layer 3 - Network

- IP spoofing
- Routing attacks
- Network scanning

Layer 4 - Transport

- Port scanning
- TCP-related attacks
- UDP-related attacks

Layer 7 - Application

- SQL injection
- Cross-site scripting
- HTTP attacks

Understanding the layer helps security professionals understand where a problem or attack is occurring.

---

# 14. OSI Memory Trick

From Layer 7 to Layer 1:

All People Seem To Need Data Processing

A - Application
P - Presentation
S - Session
T - Transport
N - Network
D - Data Link
P - Physical

From Layer 1 to Layer 7:

Please Do Not Throw Sausage Pizza Away

P - Physical
D - Data Link
N - Network
T - Transport
S - Session
P - Presentation
A - Application

---

# 15. Important Concepts to Remember

Layer 7:

Application

Layer 6:

Presentation

Layer 5:

Session

Layer 4:

Transport → TCP / UDP

Layer 3:

Network → IP

Layer 2:

Data Link → MAC

Layer 1:

Physical → Cables / Signals

---

# 16. What I Learned

Today I learned:

- What the OSI model is
- The 7 OSI layers
- Application layer
- Presentation layer
- Session layer
- Transport layer
- Network layer
- Data Link layer
- Physical layer
- TCP and UDP
- IP addresses
- MAC addresses
- Packets
- Frames
- Segments
- Bits
- How the OSI model relates to cybersecurity

## Day 2 Networking Result

I can now identify the 7 OSI layers and understand the basic purpose of each layer.
