# ISO's OSI  Layers Overview

This is my attempt to update myself and fellow connection about ISO OSI layer

## Layer 7: Application Layer

The Application Layer is the topmost layer responsible for providing services directly to end-user applications. It facilitates communication between applications and users, ensuring user requests are transmitted over the network.

**Key Protocols Used**:
- **HTTP/HTTPS**: For web browsing.
- **SMTP/POP3/IMAP**: For email communication.
- **FTP/SFTP**: For file transfers.

---

## Layer 6: Presentation Layer

The Presentation Layer is responsible for data translation, encryption, and compression. It ensures that data is presented in a readable format for the Application Layer by managing how the data is structured (syntax) and what it means (semantics).

**Key Functions**:
- Data format conversion (e.g., any to ASCII).
- Encryption/decryption (e.g., SSL/TLS).
- Data compression (e.g., JPEG, MPEG).

---

## Layer 5: Session Layer

The Session Layer manages the session between applications, establishing, maintaining, and terminating connections. It ensures sessions are synchronized, handles dialogue control, and manages session recovery in case of disruptions.

**Key Functions**:
- Session establishment, maintenance, and termination.
- Allowing sessions to resume after interruption using checkpoints.

**Key Protocols**:
- **RPC (Remote Procedure Call)**: Executes procedures/commands on remote hosts.
- **NetBIOS**: Provides sessions between networked computers.

---

## Layer 4: Transport Layer

The Transport Layer is responsible for reliable data transfer between devices. It handles error detection, correction, and flow control to ensure data is delivered in the correct order.

**Key Protocols**:
- **TCP (Transmission Control Protocol)**: Connection-oriented protocol for reliable delivery.
- **UDP (User Datagram Protocol)**: Connectionless protocol for faster delivery but less reliable transmission.

---

## Layer 3: Network Layer

The Network Layer handles routing and forwarding of packets across multiple networks. It determines the best path for data transmission based on network conditions and uses logical addressing (IP addresses).

**Key Protocols**:
- **IP (Internet Protocol)**: Primary protocol for routing packets.
- **ICMP (Internet Control Message Protocol)**: Used for diagnostics and error handling.

**Examples**:
- **Ping**: Uses ICMP to check connectivity.
- **Traceroute**: Checks the path packets take to reach their destination by sending packets with increasing TTL and recording responses from each router.
**Data**: Packets (containing data and IP addressing information).


---

## Layer 2: Data Link Layer

The Data Link Layer is responsible for node-to-node data transfer and error detection within a local network. It uses MAC addresses to identify devices within the same local network segment and ensures data frames are properly addressed and transmitted over the physical network.

**Key Functions**:
- Framing: Encapsulating packets into frames.
- Use of MAC addresses to uniquely identify devices in a network.

Data: Frames (e.g., Ethernet frames).

---

## Layer 1: Physical Layer

The Physical Layer deals with the physical aspects of data transmission over network media, including cables, switches, and NIC cards. It focuses on sending raw bits over a physical medium like cables or fiber, represented by electrical, optical, or radio signals.

**Key Functions**:
- Enables connection between devices for data transmission over physical connections.

**Data**: Bits (binary 1s and 0s, in electrical, optical, or radio form).


**Example**:
- **RS-232**: Used to connect computers and their peripherals, such as modems and printers, allowing them to communicate.

---

+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

# TCP/IP Model Overview

This document provides an overview of the layers in the TCP/IP model, detailing the functions and key protocols associated with each layer.

## Layer 4: Application Layer

The Application Layer encompasses protocols that directly interact with end-user applications. It provides network services to applications and facilitates communication between applications and users.

**Key Protocols Used**:
- **HTTP/HTTPS**: For web browsing.
- **FTP/SFTP**: For file transfers.
- **SMTP/POP3/IMAP**: For email communication.
- **DNS**: For domain name resolution.

---

## Layer 3: Transport Layer

The Transport Layer ensures reliable data transfer between devices and manages end-to-end communication. It handles error detection, correction, and flow control to ensure data is delivered in the correct order.

**Key Protocols**:
- **TCP (Transmission Control Protocol)**: Connection-oriented protocol that provides reliable delivery.
- **UDP (User Datagram Protocol)**: Connectionless protocol that allows faster delivery but with less reliability.

---

## Layer 2: Internet Layer

The Internet Layer is responsible for addressing and routing packets across networks. It determines the best path for data transmission based on network conditions and uses logical addressing (IP addresses).

**Key Protocols**:
- **IP (Internet Protocol)**: The primary protocol for routing packets.
- **ICMP (Internet Control Message Protocol)**: Used for diagnostics and error handling.
- **ARP (Address Resolution Protocol)**: Resolves IP addresses to MAC addresses.

**Examples**:
- **Ping**: Uses ICMP to check connectivity.
- **Traceroute**: Analyzes the path packets take to their destination by sending packets with increasing TTL.

---

## Layer 1: Network Interface Layer

The Network Interface Layer deals with the physical network hardware and protocols used to connect to the network. It is responsible for node-to-node data transfer and error detection within a local network.

**Key Functions**:
- Framing: Encapsulating packets into frames for transmission.
- Use of MAC addresses to uniquely identify devices within the same local network segment.

**Key Protocols**:
- **Ethernet**: Commonly used for wired LAN connections.
- **Wi-Fi**: Used for wireless networking.

---