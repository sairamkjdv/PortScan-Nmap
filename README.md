# Task 1 – Network Port Scanning using Nmap

## Objective
To perform basic network reconnaissance and identify open ports on devices within the local network using **Nmap**.

---

## Tools Used
- **Nmap** – for port scanning
- **CMD (Command Prompt)** – to check IP configuration
- **Windows 10 OS**

---

##  My Network Info
- **Local IP:** 192.168.31.186
- **IP Range Scanned:** 192.168.31.0/24

---

## Scan Results

### Host 1: `192.168.31.1` (likely the router)
- Open Ports:
  - `23` – Telnet (Insecure)
  - `53` – DNS
  - `80` – HTTP
  - `443` – HTTPS
  - `8192`, `8193`, `8383`, `8899` – Unknown/Custom services

### Host 2: `192.168.31.186` (my system)
- Open Ports:
  - `135`, `139`, `445` – Microsoft RPC/SMB Services

---

## Screenshots
![IP Configuration](./ipconfig.png)  
![Nmap Scan](./nmap_scan.png)

---

##  Security Insight
- Port `23` (Telnet) is insecure and should be disabled on the router.
- Ports `135`, `139`, `445` are commonly targeted in SMB vulnerabilities.
- Custom services (8192–8899) could be potential attack surfaces if misconfigured.

---

## Learning Outcomes
- Understood IP ranges and subnetting
- Performed TCP SYN scans using Nmap
- Analyzed exposed services
- Learned how open ports pose potential risks

---

> Task completed as part of Elevate Labs Cyber Security Internship Program.
