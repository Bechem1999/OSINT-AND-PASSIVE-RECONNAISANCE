# 🔐 Day 01 — OSINT & Passive Reconnaissance

![Internship](https://img.shields.io/badge/Internship-Sqrock%20IT%20Solution-blue)
![Day](https://img.shields.io/badge/Day-01-green)
![Project](https://img.shields.io/badge/Project-OSINT%20%26%20Passive%20Reconnaissance-orange)
![Python](https://img.shields.io/badge/Python-3.x-yellow?logo=python)
![Kali Linux](https://img.shields.io/badge/Kali%20Linux-2026.2-blue?logo=kalilinux)
![VirtualBox](https://img.shields.io/badge/VirtualBox-7.2-blue?logo=virtualbox)
![Status](https://img.shields.io/badge/Status-Completed-success)

> **SQROCK IT Solution — 15-Day Cybersecurity Internship**  
> **Day 01: OSINT & Passive Reconnaissance**

---

## 📌 1. Project Overview

This project is **Day 01** of the SQROCK IT Solution 15-Day Cybersecurity Internship.

The project focuses on **Open-Source Intelligence (OSINT)** and **passive reconnaissance**. The objective is to understand how publicly available information can be collected and analyzed without directly interacting with or attacking a target system.

A Python-based OSINT scanner was developed to automate the collection of basic information from a practice domain, including:

* WHOIS information
* DNS and IP address information
* IP geolocation information
* Basic domain intelligence

The project was conducted in a controlled cybersecurity laboratory environment for educational purposes.

---

## 🎯 2. Objectives

The main objectives of this project were to:

* Understand the fundamentals of **Open-Source Intelligence (OSINT)**.
* Understand the difference between **passive and active reconnaissance**.
* Learn how publicly available information can be used during reconnaissance.
* Perform basic **WHOIS information gathering**.
* Perform **DNS and IP address resolution**.
* Retrieve basic **IP geolocation information**.
* Develop a Python script to automate OSINT information gathering.
* Practice documenting cybersecurity activities professionally.
* Conduct reconnaissance activities only within an authorized learning environment.

---

## 🛠️ 3. Tools and Technologies Used

| Tool / Technology     | Purpose                                   |
| --------------------- | ----------------------------------------- |
| 🐍 Python 3.x         | Development of the OSINT scanner          |
| 🐉 Kali Linux         | Cybersecurity laboratory operating system |
| 💻 VirtualBox         | Virtualization and laboratory environment |
| 🔎 WHOIS              | Domain registration information gathering |
| 🌐 DNS                | Domain-to-IP resolution                   |
| 📡 Python Socket      | DNS/IP resolution                         |
| 🌍 IP Geolocation API | Basic geographic information about an IP  |
| 📦 Requests           | HTTP requests to the geolocation service  |
| 📝 Git & GitHub       | Project documentation and version control |
| 🖥️ Nano              | Python script and documentation editing   |

### Python Libraries

```text
whois
requests
socket
```

---

## 💡 4. Skills Demonstrated

This project demonstrates practical skills in:

### 🔎 Reconnaissance & OSINT

* Open-source intelligence gathering
* Passive reconnaissance
* Domain information gathering
* DNS reconnaissance
* IP address identification
* Basic IP geolocation analysis

### 🐍 Python

* Python scripting
* Importing and using external libraries
* Functions
* Exception handling
* Network-related Python operations
* HTTP requests
* Processing API responses

### 🛡️ Cybersecurity

* Reconnaissance methodology
* Information gathering
* Security awareness
* Ethical cybersecurity practices
* Controlled laboratory testing

### 📝 Documentation

* Technical documentation
* GitHub README development
* Command-line evidence collection
* Project organization
* Cybersecurity report writing

---

## 🔬 5. Methodology

The project followed a structured passive reconnaissance methodology.

### Step 1 — Select a Practice Domain

A practice domain was selected for the exercise.

The project avoids unauthorized reconnaissance against real individuals, organizations, or systems.

<img width="805" height="554" alt="week 1 project, creating a python virtual environment" src="https://github.com/user-attachments/assets/0c9436b9-e13b-4213-9b30-e2960f2164f8" />


### Step 2 — Perform WHOIS Lookup

WHOIS information was gathered to identify publicly available domain registration information.

Example:

```bash
whois example.com
```

The Python scanner also performs this operation automatically.

<img width="686" height="534" alt="installing python whois" src="https://github.com/user-attachments/assets/27f3a273-14fe-4b70-98a7-27c816ed717b" />



### Step 3 — Perform DNS Resolution

The domain was resolved to its corresponding IP address.

Example:

```bash
nslookup example.com
```

Python's `socket` module was also used:

```python
socket.gethostbyname(domain)
```

<img width="674" height="522" alt="testing DNS resolution manually" src="https://github.com/user-attachments/assets/352f383a-3980-4f5c-a12b-b9ea7b7304ef" />


### Step 4 — Retrieve IP Geolocation Information

After obtaining the IP address, the Python script sends a request to an IP geolocation service to retrieve basic information such as:

* Country
* Region
* City
* ISP

<img width="767" height="401" alt="IP GEOLOCATION" src="https://github.com/user-attachments/assets/26117c0f-6e93-41b4-8563-9c08fe945592" />


### Step 5 — Automate the Process

A Python-based OSINT scanner was created to combine the reconnaissance activities into one automated workflow.

The scanner follows this sequence:

```text
Practice Domain
      │
      ▼
   WHOIS
      │
      ▼
 DNS Resolution
      │
      ▼
  IP Address
      │
      ▼
IP Geolocation
      │
      ▼
Formatted Results
```

<img width="627" height="433" alt="OSINT python script created and run" src="https://github.com/user-attachments/assets/06826244-fecd-400d-8a1d-8edbb2226789" />



### Step 6 — Save the Results

The scanner output was saved for documentation and analysis.

```bash
python3 osint_scan.py | tee output.txt
```

<img width="810" height="449" alt="OSINT output saved in  txt format" src="https://github.com/user-attachments/assets/6dee4d49-42f6-43ee-bd31-fb49703feecc" />



### Step 7 — Document the Findings

Screenshots, command outputs, code, and observations were documented as part of the project deliverables.

---

## 🧪 6. Laboratory Environment

The project was conducted within a controlled virtual cybersecurity laboratory.

### Laboratory Platform

```text
Host Computer
      │
      ▼
VirtualBox
      │
      ▼
Kali Linux VM
      │
      ▼
Private NAT Network
10.0.0.0/24
```

### Virtual Laboratory Components

| Component               | Configuration     |
| ----------------------- | ----------------- |
| Virtualization Platform | VirtualBox 7.2    |
| Operating System        | Kali Linux 2026.2 |
| Network Type            | NAT Network       |
| Network Name            | NatNetwork        |
| IPv4 Network            | 10.0.0.0/24       |
| DHCP                    | Enabled           |
| IPv6                    | Disabled          |

The laboratory provides a controlled environment for cybersecurity learning and authorized testing.

---

## ⚙️ 7. Environment Configuration

### VirtualBox Network Configuration

The VirtualBox NAT Network was configured with:

```text
Network Name: NatNetwork
IPv4 Prefix: 10.0.0.0/24
DHCP Enabled: Yes
IPv6: Disabled
```

The NAT Network configuration allows virtual machines connected to the same virtual network to communicate while maintaining outbound network connectivity.

### Kali Linux Configuration

The Kali Linux virtual machine was configured with network connectivity through the VirtualBox NAT Network.

Network connectivity was verified using:

```bash
ip a
```

Gateway connectivity:

```bash
ping -c 4 10.0.0.1
```

Internet connectivity:

```bash
ping -c 4 8.8.8.8
```

DNS connectivity:

```bash
ping -c 4 example.com
```

DNS resolution was also tested with:

```bash
nslookup example.com
```

### Python Environment

The required Python libraries were installed before running the scanner:

```bash
pip install python-whois requests
```

Where necessary, a Python virtual environment was used to avoid conflicts with the system Python environment.

---

## 📁 8. Project Structure

The project was organized as follows:

```text
Day01_OSINT/
│
├── osint_scan.py
├── output.txt
├── README.md
├── Day01_Report.md
├── Day01_OSINT_Result.png
└── Day01_OSINT_Code.png
```

### File Description

| File                     | Description                                  |
| ------------------------ | -------------------------------------------- |
| `osint_scan.py`          | Python OSINT scanner                         |
| `output.txt`             | Saved scanner results                        |
| `README.md`              | Project documentation                        |
| `Day01_Report.md`        | Detailed project report                      |
| `Day01_OSINT_Result.png` | Screenshot of scanner execution              |
| `Day01_OSINT_Code.png`   | Screenshot showing the Python implementation |

---

## 📚 9. Learning Outcomes

At the completion of this project, I gained practical experience in:

* Understanding OSINT concepts.
* Understanding passive reconnaissance techniques.
* Performing basic WHOIS reconnaissance.
* Performing DNS and IP resolution.
* Collecting basic IP geolocation information.
* Automating reconnaissance tasks using Python.
* Working with Python networking libraries.
* Working with external APIs.
* Handling errors in Python scripts.
* Organizing cybersecurity projects.
* Documenting technical findings.
* Using GitHub as a cybersecurity portfolio platform.
* Applying ethical principles when conducting reconnaissance.

---

## ⚠️ 10. Challenges Faced and How They Were Overcome

### Challenge 1 — Installing Python Dependencies

One challenge was installing external Python libraries such as `python-whois` and `requests` in the Kali Linux environment.

**Solution:**

A Python virtual environment can be created to isolate project dependencies:

```bash
python3 -m venv venv
source venv/bin/activate
pip install python-whois requests
```

This provides an isolated environment for the project dependencies.

---

### Challenge 2 — DNS Resolution

DNS resolution can fail when there is a network or DNS configuration problem.

**Solution:**

DNS connectivity was tested independently using:

```bash
nslookup example.com
```

and:

```bash
ping -c 4 example.com
```

This helped distinguish between a Python problem and an underlying network/DNS problem.

---

### Challenge 3 — Network Connectivity

Before running the OSINT scanner, network connectivity needed to be verified.

**Solution:**

Connectivity was tested at multiple levels:

```bash
ping -c 4 10.0.0.1
```

followed by:

```bash
ping -c 4 8.8.8.8
```

and finally:

```bash
ping -c 4 example.com
```

This helped verify the gateway, Internet connection, and DNS resolution separately.

---

### Challenge 4 — Handling Lookup Errors

WHOIS and IP geolocation services may sometimes return incomplete information or fail to respond.

**Solution:**

Python exception handling was implemented using `try` and `except` blocks so that the scanner could report errors without terminating unexpectedly.

Example:

```python
try:
    w = whois.whois(domain)
except Exception as error:
    print(f"WHOIS lookup failed: {error}")
```

---

### Challenge 5 — Organizing Project Evidence

Another challenge was maintaining the code, output, screenshots, and documentation in an organized manner.

**Solution:**

A dedicated project directory was created with separate files for the Python implementation, output, report, and screenshots.

This makes the project easier to review, reproduce, and publish on GitHub.

---

## ✅ Project Status

**Status:** Completed ✅

### Key Deliverables

* ✅ Python OSINT scanner
* ✅ WHOIS information gathering
* ✅ DNS/IP resolution
* ✅ IP geolocation lookup
* ✅ Saved scanner output
* ✅ Technical documentation
* ✅ Project report
* ✅ Screenshots and evidence
* ✅ Organized GitHub project structure

---

## 🔐 Ethical Considerations

This project was conducted strictly for **educational and authorized cybersecurity training purposes**.

The reconnaissance activities were limited to practice/laboratory targets. No attempt was made to:

* Access unauthorized systems
* Obtain private credentials
* Attack external infrastructure
* Exploit vulnerabilities
* Conduct intrusive scanning
* Interact with real users or employees

The purpose of the exercise was to understand how publicly available information can be collected and how OSINT can contribute to cybersecurity reconnaissance

## 🚀 Conclusion

Day 01 provided practical experience with **OSINT and passive reconnaissance** using a controlled cybersecurity laboratory environment.

The project demonstrated how Python can be used to automate basic information-gathering activities while reinforcing the importance of authorization, responsible reconnaissance, and professional cybersecurity documentation.

This project forms the foundation for subsequent cybersecurity internship tasks involving security awareness, detection, analysis, and controlled security simulations.


 # 👤 Author
  Atemlefac Nkafu Bechem
  
  Cybersecurity Engineer

LinkedIn: https://www.linkedin.com/in/atemlefac-nkafu-bechem-179987248

# 📌 Project Information
**Program Name:** Cybersecurity at SQROCK | **Week:** 01 | **Project:** OSINT and passive reconnaisance | **Repository:** GitHub
