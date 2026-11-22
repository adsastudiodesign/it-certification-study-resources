# CompTIA Security+ Domain Checklist

The whole Security+ field, organised by the exam's five domains. Tick a topic only when you can explain it out loud, from memory — and, for scenario-heavy domains, say what you would *do* with it on the job.

## Domain 1 — General Security Concepts

- [ ] The CIA triad: confidentiality, integrity, availability — and a real example of each failing
- [ ] AAA: authentication, authorisation, accounting — and how a RADIUS/TACACS+ login walks through all three
- [ ] Zero trust: control plane vs data plane, policy engine, policy administrator, policy enforcement point
- [ ] Security controls by category: technical, managerial, operational, physical
- [ ] Security controls by type: preventive, detective, corrective, compensating, deterrent, directive
- [ ] Cryptography basics: symmetric vs asymmetric, hashing, digital signatures, certificates and PKI at concept level
- [ ] Threat actors: nation-state, hacktivist, insider, organised crime, shadow IT — resources, funding, sophistication
- [ ] Physical controls: sensors, locks, fencing, bollards, access badges, Faraday cages

**Acronyms to own in this domain:** CIA · AAA · PKI · CA · CRL · OCSP · HSM · TPM · DLP

## Domain 2 — Threats, Vulnerabilities & Attacks

- [ ] Malware: ransomware, trojans, worms, viruses, keyloggers, logic bombs, rootkits, fileless malware
- [ ] Social engineering: phishing, spear phishing, whaling, vishing, smishing, pretexting, watering hole, brand impersonation, influence campaigns
- [ ] Application attacks: injection (SQL, LDAP, XML), XSS, CSRF, privilege escalation, directory traversal, API attacks, replay and pass-the-hash
- [ ] Network attacks: DDoS, DNS poisoning, ARP poisoning, on-path (man-in-the-middle), evil twin, jamming, Bluetooth attacks (bluejacking, bluesnarfing)
- [ ] Vulnerability management: scanning vs penetration testing, credentialed vs non-credentialed scans, CVE and CVSS, false positives and negatives
- [ ] Threat intelligence: OSINT, threat feeds, MITRE ATT&CK, the dark web's role in intelligence
- [ ] Password attacks: brute force, spraying, dictionary, rainbow tables, credential stuffing

**Acronyms to own in this domain:** CVE · CVSS · OSINT · DDoS · XSS · CSRF · SQLi · APT

## Domain 3 — Security Architecture

- [ ] Network design: segmentation, microsegmentation, VLANs, VPNs, jump servers, air gaps, port security (802.1X, EAP)
- [ ] Secure protocols and their ports: HTTPS, SFTP, FTPS, LDAPS, DNSSEC, SRTP, SNMPv3 — and the insecure versions they replace
- [ ] Cloud security: shared responsibility, CASB, SASE, cloud access security, resource policies, secrets management
- [ ] Identity architecture: federation, SSO, SAML, OAuth, OpenID Connect, MFA methods and their weaknesses
- [ ] Cryptography in depth: AES, RSA, ECC, Diffie-Hellman, key exchange, key escrow, salting, hashing algorithms (SHA family), digital envelopes
- [ ] Data protection: data states (at rest, in transit, in use), encryption, tokenisation, masking, data classification, retention and disposal
- [ ] Resilience: load balancers, clustering, backups (full, incremental, differential), snapshots, RAID, UPS and generators, site types (hot, warm, cold)
- [ ] Embedded and IoT security: constraints of embedded systems, RTOS, securing ICS/SCADA environments

**Acronyms to own in this domain:** CASB · SASE · SSO · SAML · MFA · EAP · AES · ECC · RAID · RTO · RPO

## Domain 4 — Security Operations

- [ ] Identity and access management on the job: provisioning and deprovisioning, account audits, permission assignments, password policies
- [ ] Hardening: OS baselines, group policies, disabling unnecessary services, endpoint protection (EDR/XDR, DLP, HIDS/HIPS, NGFW)
- [ ] Monitoring and alerting: SIEM, SOAR, log management, NetFlow, packet capture, alert tuning and baselining
- [ ] Incident response process, in order: preparation, detection, analysis, containment, eradication, recovery, lessons learned
- [ ] Digital forensics: legal hold, chain of custody, acquisition, and the order of volatility (cache → RAM → disk → logs → archival media)
- [ ] Automation and orchestration in security operations: scripting use cases and their guardrails
- [ ] Asset management: hardware and software inventories, assignment, monitoring, and disposal/sanitisation (wipe, purge, clear, destruction)

**Acronyms to own in this domain:** SIEM · SOAR · EDR · XDR · DLP · HIDS · HIPS · NGFW · UEBA

## Domain 5 — Security Program Management & Oversight

- [ ] Risk management: risk assessment (qualitative vs quantitative), risk register, risk matrix, likelihood and impact, risk handling (accept, mitigate, transfer, avoid)
- [ ] The arithmetic: SLE, ARO, ALE (ALE = SLE × ARO), exposure factor
- [ ] Business impact analysis: RTO, RPO, MTBF, MTTR — and telling them apart under pressure
- [ ] Governance: policies, standards, procedures, guidelines — in that hierarchy; roles of the board, CISO, and data owners/custodians
- [ ] Compliance: GDPR, PCI DSS, HIPAA in outline; compliance monitoring, due diligence, and attestation
- [ ] Audits and assessments: internal vs external audits, penetration test rules of engagement, attestation vs audit
- [ ] Vendor management: MSA, SLA, MOUs, supply-chain risk, right-to-audit clauses
- [ ] Security awareness: training programs, phishing campaigns, reporting culture

**Acronyms to own in this domain:** SLE · ARO · ALE · BIA · RTO · RPO · MTBF · MTTR · SLA · MSA

---

*This checklist is part of the free study resources from **Mastering Careers & Skills**, drawn from the structure of our complete book **IT Security Certificate (CompTIA Security+)** — the complete IT security course, teaching all five domains from the ground up. **Read Chapter 1 free:** https://careersskillsbooks.com/book/security-plus/*

*An independent study resource. Not affiliated with, sponsored by, or endorsed by CompTIA.*
