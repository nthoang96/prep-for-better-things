## Concept
### Core Physical & Local Connections
**Ethernet & Wifi**
- Ethernet is wired - a cable (with a Registered Jack 45 - RJ45) running from the device to a switch or router. It's fast and stable.
- Wifi does the same job wirelessly over radio waves, more convenient, but more prone to interference.

**MAC Address** - Media Access Control
- Is the unique hardware ID baked into every network interface (laptop's Wifi card, phone, a printer, each has its own). It's a 48-bit value written like `00:1A:2B:3C:4D:5E`. This is how devices identify each other on the same local network.

**Switch**
- Is the box that ties the local network together. Multiple devices plug into it (or connect to it via Wifi through a router). It reads destination MAC addresses to forward data packets only to the intended device.

![[switch.png]]

### Network Identification & Sizing
**IP Address**
- A logical, changeable address assigned to a device so it can be identified across different networks.
	- **Static IP**: Manually typed and assigned in network settings.
	- **DHCP** - Dynamic Host Configuration Protocol: Automatically assigns IP addresses to devices when they join a network. 

**Subnet**
- A parameter that defines the specific size (boundaries) of your local network.

### Routing Traffic Between Networks
**Router**
- The "exit door" of a local network. It connects different networks together by looking at destination IP addresses and deciding where to send the data next.

**Default Gateway**
- The specific router your device sends traffic to when it doesn't know where a destination IP is located.

**Routing Protocols**
Rules that tell routers where to forward traffic:
- Static Routing - manually configured paths, ideal only for small networks
- Dynamic Routing
	- IGP - Interior gateway: run within a single organization's network
		- OSPF (Open Shortest Path First): Automatically finds the best paths for routers communicating inside a single organization.
	- EGP - Exterior gateway: run between autonomous systems between different companies and ISPs that make up the internet.
		- BGP (Border Gateway Protocol): The protocol used by large Internet Service Providers (ISPs) to exchange routing paths between different companies.

![[routing.png]]
### Troubleshooting & Data Protocols
**Ping & ICMP**
Ping sends a small packet to a destination to check if it's reachable. It relies on ICMP (Internet Control Message Protocol) which is used primarily for network troubleshooting.

**TCP** - Transmission Control Protocol
A reliable, connection-oriented protocol. It ensures every packet arrives safely and resends lost data, making it great for file transfers but slower due to confirmation wait-times.

**UDP** - User Datagram Protocol
A fast, connectionless protocol. It sends data without waiting for arrival confirmations. If packets are lost, they are gone forever, making it ideal for live streaming, gaming, and video calls.

**Ports**
Virtual numbers that direct data to the correct application on a device once the IP address finds the correct hardware (port 80 for HTTP, 443 for HTTPS, 53 for DNS, 22 for SSH, 25 for SMTP).
![[network-trouble-shooting.png]]
### Network Security
![[network-security.png]]**Firewall**
A barrier that controls incoming and outgoing traffic based on security rules, capable of blocking specific ports or IP addresses.

**TLS** - Transport Layer Security
The modern successor to SSL. It encrypts a specific connection (like a web browser to a server) to prevent bad actors from reading data in plain text.

**VPN** - Virtual Private Network
Creates a fully encrypted tunnel that protects all network traffic leaving your device to another network, ensuring privacy.

![[vpn.png]]

### Web Interaction & Scaling
**DNS** - Domain Name System
The internet's phonebook. It translates human-readable domain names (like `google.com`) into computer-readable IP addresses.

**HTTP & HTTPS**
HTTP is the protocol browsers use to request and load web pages. Combining HTTP with TLS encryption yields HTTPS.

**Load Balancer**
A device sitting in front of multiple servers that distributes incoming user requests evenly among them. This prevents server overloads and ensures application uptime.