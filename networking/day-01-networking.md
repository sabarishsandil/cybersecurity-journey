# Day 1 - Networking

## 1. What is Networking?

Networking is the process of connecting computers and other devices so they can communicate and share information.

Examples:
- Computers connected in a college lab
- Phones connected to Wi-Fi
- Servers communicating over the Internet

Networking is very important in cybersecurity because attackers and defenders both interact with networks.

---

## 2. What is the Internet?

The Internet is a global network of interconnected computers and devices that communicate using standard networking protocols.

When we access a website:

1. Our device sends a request.
2. DNS helps find the server's IP address.
3. The request travels through networks and routers.
4. The server processes the request.
5. The server sends data back to our device.
6. The browser displays the website.

Important components include:

- Client
- Server
- Router
- ISP
- Protocols
- IP addresses

---

## 3. Client

A client is a device or application that requests a service from a server.

Examples:

- Web browser
- Mobile phone
- Laptop
- Email application

Example:

When I open a website, my browser acts as a client.

---

## 4. Server

A server is a computer or system that provides services or resources to clients.

Examples:

- Web server
- Database server
- DNS server
- Mail server
- File server

Example:

When I open a website, the website's server sends the requested data to my browser.

---

## 5. Router

A router connects different networks and forwards packets between them.

For example:

My laptop
    |
Wi-Fi Router
    |
ISP
    |
Internet
    |
Website Server

Routers help determine where network traffic should go.

---

## 6. ISP

ISP stands for Internet Service Provider.

An ISP provides Internet access to customers.

Examples of services provided by ISPs:

- Internet connectivity
- IP address assignment
- DNS services
- Broadband connections

---

# 7. LAN

LAN stands for Local Area Network.

A LAN connects devices within a relatively small geographical area.

Examples:

- Home network
- College computer lab
- Office network
- School network

Characteristics:

- Small geographical area
- Generally high speed
- Low latency
- Usually privately managed

Example:

Laptop
   |
Wi-Fi Router
   |
Phone
   |
Printer

All these devices can communicate through the local network.

---

# 8. WAN

WAN stands for Wide Area Network.

A WAN connects networks over large geographical areas.

Examples:

- Network connecting company branches
- Banking networks
- The Internet

Characteristics:

- Large geographical coverage
- Connects multiple LANs
- Usually more complex than LAN
- Can have higher latency than LAN

---

# 9. LAN vs WAN

| Feature | LAN | WAN |
|---|---|---|
| Full Form | Local Area Network | Wide Area Network |
| Coverage | Small area | Large area |
| Speed | Generally higher | Generally lower |
| Latency | Usually lower | Usually higher |
| Example | Home network | Internet |
| Connection | Local devices | Multiple networks |

---

# 10. IP Address

IP stands for Internet Protocol.

An IP address is a numerical address used to identify a device or network interface and enable communication using the Internet Protocol.

Example:

192.168.1.10

An IP address helps network traffic reach the correct destination.

Think of it like a postal address:

House Address → identifies a house
IP Address → identifies a network interface

---

# 11. Public IP Address

A public IP address is an address used for communication across the Internet.

It is generally assigned by an Internet Service Provider.

Example:

203.0.113.10

Public IP addresses need to be globally routable and are not normally used by multiple unrelated devices at the same time.

---

# 12. Private IP Address

Private IP addresses are used inside private networks such as homes, schools, and offices.

Common private IPv4 ranges are:

10.0.0.0/8

172.16.0.0/12

192.168.0.0/16

Example:

192.168.1.10

Private addresses are not directly routable across the public Internet.

A router commonly uses NAT to allow devices with private addresses to communicate with Internet services.

---

# 13. IPv4

IPv4 stands for Internet Protocol version 4.

IPv4 uses 32-bit addresses.

Example:

192.168.1.1

An IPv4 address contains four decimal numbers separated by dots.

Example:

192 . 168 . 1 . 1

Each part can range from 0 to 255.

IPv4 provides approximately 4.3 billion possible addresses.

---

# 14. IPv6

IPv6 stands for Internet Protocol version 6.

IPv6 uses 128-bit addresses.

Example:

2001:db8:85a3::8a2e:370:7334

IPv6 uses hexadecimal numbers separated by colons.

IPv6 was introduced mainly to provide a much larger address space than IPv4.

Advantages include:

- Very large address space
- Efficient address allocation
- Better support for modern networking
- Simplified network configuration in many environments
- Reduced dependence on NAT

---

# 15. IPv4 vs IPv6

| Feature | IPv4 | IPv6 |
|---|---|---|
| Version | 4 | 6 |
| Address Size | 32-bit | 128-bit |
| Example | 192.168.1.1 | 2001:db8::1 |
| Format | Decimal | Hexadecimal |
| Address Space | About 4.3 billion | Extremely large |
| NAT | Commonly used | Usually less necessary |

---

# 16. Network Protocol

A protocol is a set of rules that devices follow to communicate with each other.

Examples:

- TCP
- UDP
- HTTP
- HTTPS
- DNS
- SSH

Different protocols perform different jobs.

---

# 17. TCP

TCP stands for Transmission Control Protocol.

TCP provides reliable, connection-oriented communication.

It ensures that data is delivered reliably and in the correct order.

Common uses:

- HTTPS
- SSH
- Email
- File transfers

---

# 18. UDP

UDP stands for User Datagram Protocol.

UDP is connectionless and does not provide the same delivery guarantees as TCP.

It is useful when speed and low overhead are more important than guaranteed delivery.

Common uses include:

- DNS
- Streaming
- Online gaming
- Voice/video communication

---

# 19. DNS

DNS stands for Domain Name System.

DNS translates domain names into IP addresses.

Example:

google.com
     |
    DNS
     |
IP address

Instead of remembering an IP address, users can type:

google.com

DNS helps find the corresponding server address.

---

# 20. HTTP

HTTP stands for Hypertext Transfer Protocol.

It is commonly used for communication between web browsers and web servers.

Example:

Browser
   |
HTTP Request
   |
Web Server
   |
HTTP Response
   |
Browser

---

# 21. HTTPS

HTTPS stands for Hypertext Transfer Protocol Secure.

HTTPS uses encryption through TLS to protect data exchanged between a client and server.

It helps protect against:

- Eavesdropping
- Data modification
- Certain man-in-the-middle attacks

Example:

https://example.com

---

# 22. Ports

A port is a logical communication endpoint used by network services.

Examples of commonly associated ports:

| Port | Common Service |
|---|---|
| 22 | SSH |
| 53 | DNS |
| 80 | HTTP |
| 443 | HTTPS |

Ports help a computer distinguish between different network services.

Example:

Server IP: 192.168.1.10
Port: 443

This indicates a service listening on TCP port 443.

---

# 23. Packets

Network data is commonly divided into smaller units called packets.

A packet can contain:

- Source information
- Destination information
- Protocol information
- Data

Example:

Computer A
    |
    | Packet
    v
Router
    |
    v
Server

Routers examine packet information to determine where to forward traffic.

---

# 24. Why Networking is Important in Cybersecurity

Understanding networking is essential for cybersecurity.

It helps with:

- Network security
- Penetration testing
- Vulnerability assessment
- Packet analysis
- Firewall configuration
- Intrusion detection
- Incident response
- Malware analysis
- Web security

Tools that we will learn later include:

- Nmap
- Wireshark
- Burp Suite
- Netcat

---

# 25. What I Learned Today

Today I learned:

- What networking is
- What the Internet is
- Client and server
- Routers
- ISP
- LAN
- WAN
- IP addresses
- Public IP
- Private IP
- IPv4
- IPv6
- TCP
- UDP
- DNS
- HTTP
- HTTPS
- Ports
- Packets

I also learned why networking knowledge is important for cybersecurity.

---

# Next Networking Topics

I will learn these topics in the following days:

- OSI Model
- TCP/IP Model
- MAC Address
- ARP
- DHCP
- NAT
- Subnetting
- TCP 3-Way Handshake
- DNS in more detail
- HTTP requests and responses
- Firewalls
- VPN
