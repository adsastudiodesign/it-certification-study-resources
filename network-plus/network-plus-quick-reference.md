# CompTIA Network+ Quick Reference — Ports, the OSI Model & Subnetting

The three tables Network+ candidates are expected to carry in their heads. Revise them daily in the last week before your sitting.

## 1. Ports & protocols you must know cold

| Port | Service | Transport | What it does |
|---|---|---|---|
| 20/21 | FTP | TCP | File transfer (20 = data, 21 = control) — plaintext |
| 22 | SSH | TCP | Secure remote shell; also SFTP and SCP |
| 23 | Telnet | TCP | Remote shell — plaintext, avoid |
| 25 | SMTP | TCP | Sending mail between servers |
| 53 | DNS | UDP/TCP | Name resolution (UDP for queries, TCP for zone transfers) |
| 67/68 | DHCP | UDP | Automatic IP assignment (67 = server, 68 = client) |
| 69 | TFTP | UDP | Trivial file transfer — no authentication |
| 80 | HTTP | TCP | Web traffic — plaintext |
| 110 | POP3 | TCP | Mail retrieval (downloads to one device) |
| 123 | NTP | UDP | Time synchronisation |
| 143 | IMAP | TCP | Mail access (mail stays on the server) |
| 161/162 | SNMP | UDP | Network device monitoring (161 = queries, 162 = traps) |
| 389 | LDAP | TCP/UDP | Directory services — plaintext |
| 443 | HTTPS | TCP | Web traffic over TLS |
| 445 | SMB | TCP | Windows file and printer sharing |
| 514 | Syslog | UDP | Log forwarding to a central collector |
| 636 | LDAPS | TCP | Directory services over TLS |
| 993 | IMAPS | TCP | IMAP over TLS |
| 995 | POP3S | TCP | POP3 over TLS |
| 1433 | Microsoft SQL Server | TCP | Database connections |
| 1812/1813 | RADIUS | UDP | Authentication (1812) and accounting (1813) |
| 3389 | RDP | TCP | Windows Remote Desktop |
| 49 | TACACS+ | TCP | Cisco device administration AAA |

**The pattern that unlocks the rest:** the secure version of a service is the one the exam wants. SSH replaces Telnet, HTTPS replaces HTTP, LDAPS replaces LDAP, SFTP replaces FTP, SNMPv3 replaces v1/v2c.

## 2. The OSI model at a glance

| Layer | Name | Data unit | What lives here | Example devices / protocols |
|---|---|---|---|---|
| 7 | Application | Data | The services the user touches | HTTP, DNS, DHCP, SMTP |
| 6 | Presentation | Data | Formatting, encryption, compression | TLS, JPEG, ASCII |
| 5 | Session | Data | Opening, managing, closing conversations | RPC, NetBIOS |
| 4 | Transport | Segment | End-to-end delivery, ports | TCP, UDP |
| 3 | Network | Packet | Logical addressing, routing | IP, ICMP, routers |
| 2 | Data Link | Frame | MAC addresses, switching | Ethernet, switches, VLANs |
| 1 | Physical | Bit | Cables, signals, connectors | Copper, fibre, hubs, repeaters |

**Troubleshooting with the model:** work from the layer where the evidence points. No link light is Layer 1. A correct IP but no route is Layer 3. Connected but the application fails is Layer 7. The exam's scenarios reward naming the layer before naming the fix.

## 3. Subnetting quick table (IPv4)

| CIDR | Subnet mask | Addresses in block | Usable hosts |
|---|---|---|---|
| /24 | 255.255.255.0 | 256 | 254 |
| /25 | 255.255.255.128 | 128 | 126 |
| /26 | 255.255.255.192 | 64 | 62 |
| /27 | 255.255.255.224 | 32 | 30 |
| /28 | 255.255.255.240 | 16 | 14 |
| /29 | 255.255.255.248 | 8 | 6 |
| /30 | 255.255.255.252 | 4 | 2 |
| /31 | 255.255.255.254 | 2 | 2 (point-to-point links only) |
| /32 | 255.255.255.255 | 1 | 1 (a single host route) |

**The method, every time:**
1. Block size = 256 − the mask value in the interesting octet (for /27: 256 − 224 = 32).
2. Subnets start at multiples of the block size: 0, 32, 64, 96…
3. A host's subnet is the multiple at or just below its address; the broadcast is the next multiple minus 1.
4. Usable hosts = block size − 2 (network and broadcast), except /31 point-to-point links and /32 host routes.
5. Hosts needed → work backwards: 50 hosts needs a block of 64 → /26.

**Private address ranges (know them on sight):** 10.0.0.0/8 · 172.16.0.0/12 (172.16–172.31) · 192.168.0.0/16. **APIPA** (link-local, when DHCP fails): 169.254.0.0/16. **Loopback:** 127.0.0.1.

## Also worth a daily pass

- **Cabling:** T568A vs T568B pinouts; straight-through vs crossover; Cat 6 rated to 100 m per run; fibre is immune to EMI.
- **Wireless:** 2.4 GHz channels 1, 6, 11 are the non-overlapping set; 5 GHz has more, wider channels and shorter range; WPA3 is the current standard.
- **The troubleshooting methodology:** identify the problem → establish a theory → test → plan → implement → verify → document.

---

*This quick reference is part of the free study resources from **Mastering Careers & Skills**, drawn from the structure of our complete book **IT Network Certificate (CompTIA Network+)** — the complete networking course, from the OSI model to the arithmetic of subnetting, taught step by step. **Read Chapter 1 free:** https://careersskillsbooks.com/book/network-plus/*

*An independent study resource. Not affiliated with, sponsored by, or endorsed by CompTIA.*
