# Cisco CCNA Study Outline — with an Essential IOS Commands Quick List

A topic outline for the whole CCNA field, in study order. Tick a topic only when you can both explain it *and* picture the configuration or output that proves it on a live device.

## 1. Network fundamentals

- [ ] What routers, switches, firewalls, access points, controllers, and servers each do — and where each sits in a topology
- [ ] Topology architectures: two-tier, three-tier, spine-leaf, SOHO, WAN, and cloud
- [ ] TCP vs UDP, and which applications choose which
- [ ] Cabling: copper vs fibre, and the interface problems each one has
- [ ] IPv4 addressing and subnetting (use the method in this repo's Network+ quick reference — the arithmetic is identical)
- [ ] IPv6: address types (global unicast, unique local, link-local, multicast), prefix shortening rules, and SLAAC vs DHCPv6

## 2. Switching and network access

- [ ] How a switch learns MAC addresses and forwards frames; the MAC address table
- [ ] VLANs: access vs trunk ports, the native VLAN, inter-VLAN routing (router-on-a-stick and Layer 3 switches)
- [ ] Trunking with 802.1Q; DTP and why you disable it
- [ ] EtherChannel: PAgP vs LACP vs static, and the mismatches that stop a bundle forming
- [ ] Spanning Tree: root bridge election, port states and roles, PortFast, BPDU Guard, RSTP
- [ ] Discovery protocols: CDP and LLDP

## 3. Wireless

- [ ] WLAN components: APs, WLCs, and how lightweight APs join a controller (CAPWAP)
- [ ] RF basics: bands, channels, interference, and site surveys in outline
- [ ] WLAN configuration on a controller: SSIDs, security (WPA2/WPA3, PSK vs 802.1X), and guest access

## 4. Routing and IP connectivity

- [ ] Reading a routing table: codes, administrative distance, metric, longest-prefix match
- [ ] The forwarding decision, step by step: longest match → lowest AD → lowest metric
- [ ] Static routing: directly connected, recursive, fully specified; default routes; floating statics
- [ ] Single-area OSPFv2: neighbour formation, DR/BDR election, network types, and the configuration that makes two routers adjacent
- [ ] First-hop redundancy in outline (HSRP and family)

## 5. IP services

- [ ] DHCP: the DORA exchange, relay agents, and client configuration
- [ ] DNS and NTP: what each resolves, and why the network's clocks must agree
- [ ] NAT: static, dynamic, and PAT (overload) — and reading a translation table
- [ ] QoS in outline: classification, marking, queuing, and why voice gets priority
- [ ] SNMP and syslog: versions, traps vs polling, severity levels
- [ ] TFTP/FTP and SSH for device file management and access

## 6. Security fundamentals

- [ ] Security concepts: threats, vulnerabilities, exploits; AAA (authentication, authorisation, accounting)
- [ ] Device access security: enable secret, service password-encryption, local users, SSH-only VTY lines, login banners
- [ ] ACLs: standard vs extended, numbered vs named, wildcard masks, placement rules (standard close to the destination, extended close to the source)
- [ ] Layer 2 security: port security, DHCP snooping, dynamic ARP inspection
- [ ] VPN concepts: site-to-site vs remote access, IPsec in outline
- [ ] Wireless security: WPA2/WPA3, enterprise authentication with 802.1X and RADIUS

## 7. Automation and programmability

- [ ] Controllers and SDN: the control plane vs data plane, northbound and southbound APIs
- [ ] REST APIs in outline: verbs, status codes, CRUD
- [ ] Data formats: reading JSON and YAML well enough to parse device output
- [ ] Configuration management tools (Ansible, Terraform) and what problem each solves
- [ ] How AI and machine learning are described in network operations

## Essential IOS commands — the quick list

| Command | What it tells you / does |
|---|---|
| `show ip interface brief` | Interface status and IP addresses, one line each — the first command on any fault |
| `show running-config` | The active configuration |
| `show ip route` | The routing table |
| `show vlan brief` | VLANs and the ports assigned to them |
| `show interfaces trunk` | Which ports are trunking, and the native VLAN |
| `show etherchannel summary` | EtherChannel bundles and their state |
| `show spanning-tree` | Root bridge, port roles and states |
| `show ip ospf neighbor` | OSPF adjacencies |
| `show ip dhcp binding` | Leases the DHCP server has handed out |
| `show ip nat translations` | Live NAT/PAT translations |
| `show access-lists` | ACL entries and match counters |
| `show cdp neighbors` / `show lldp neighbors` | Directly connected devices |
| `ping` / `traceroute` | Reachability, and the path a packet takes |
| `copy running-config startup-config` | Save the configuration so it survives a reload |

---

*This outline is part of the free study resources from **Mastering Careers & Skills**, drawn from the structure of our complete book **Cisco Network Certificate (CCNA)** — the complete Cisco networking course, from networks from zero through OSPF, ACLs, and automation. **Read Chapter 1 free:** https://careersskillsbooks.com/book/ccna/*

*An independent study resource. Not affiliated with, sponsored by, or endorsed by Cisco.*
