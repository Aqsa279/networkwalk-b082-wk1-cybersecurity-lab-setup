# networkwalk-b082-wk1-cybersecurity-lab-setup
My Kali Linux cybersecurity lab setup, configuration, and hands-on documentation.

_______________________________________________________________________________________________________________________
📌 Project Overview
This project involves building a virtual cybersecurity lab using Kali Linux and VMware Workstation to develop practical skills in ethical hacking and penetration testing.

The lab provides a controlled environment for learning and practicing network configuration, reconnaissance, network scanning, vulnerability assessment, and security testing. It is designed to support hands-on experiments in a safe and organized way.

The virtual lab network can be expanded by adding more virtual machines in the future, allowing me to practice identifying security weaknesses and testing defenses on systems I own or have explicit permission to assess.


__________________________________________________________________________________________________________________
## 🎯 Project Objectives

The primary goals of this project are to build a reliable, secure, and well-organized environment for hands-on cybersecurity practice.

- 🖥️ Set up and configure VirtualBox for virtualization.
- 🐉 Install and prepare Kali Linux as the primary security-testing machine.
- 🌐 Create an isolated NAT Network for lab communication.
- ⚙️ Configure Kali Linux network settings and connectivity.
- 📡 Assign and verify the appropriate IP address for the lab environment.
- 🔎 Test network connectivity and DNS resolution.
- 💾 Create a clean virtual machine snapshot for recovery and troubleshooting.
- 📝 Document each setup stage with commands, explanations, and screenshots.

  
_____________________________________________________________________________________________________________________
## 🛡️ Lab Purpose and Applications

This virtual lab is designed to strengthen practical cybersecurity skills by providing a controlled environment for hands-on experimentation, security analysis, and ethical hacking practice.

It serves as a foundation for exploring various cybersecurity concepts and tools, including:

- 🔍 **Network Reconnaissance:** Discovering hosts and gathering network information.
- 🌐 **Port Scanning:** Identifying open ports and available services.
- 🛡️ **Vulnerability Assessment:** Finding potential security weaknesses.
- 📡 **Packet Analysis:** Examining network traffic to understand communication patterns.
- 🔐 **Web Application Security:** Practicing web security testing techniques.
- 🧪 **Penetration Testing:** Learning how to identify and validate security issues in authorized lab environments.
- ⚙️ **Security Tool Practice:** Exploring cybersecurity tools and understanding their practical applications.

### ⚠️ Ethical Use and Safety

All activities performed in this lab must remain within authorized and controlled environments. Testing should only target systems that I own or have explicit permission to assess. This ensures that cybersecurity skills are developed responsibly and ethically.

_______________________________________________________________________________________________________________________

---

## ⚙️ Lab Configuration

The following table summarizes the hardware, virtualization platform, and network settings used in my cybersecurity lab.

| **Component** | **Configuration** |
|:---|:---|
| 🖥️ Host Operating System | Windows 11 |
| 🧠 Host Memory | 16 GB RAM |
| 🧰 Virtualization Platform | VMware Workstation Pro |
| 🐉 Security Operating System | Kali Linux 2026.2 |
| 💾 Kali VM Memory | 2048 MB|
| 🌐 Virtual Network | `Nat Network` |
| 📡 Network Address |`	10.0.0.0/24` |
| 🔗 kali IP address | `10.0.0.2/24` |
| 🚪 Default Gateway | `10.0.0.1` |
| 🌍 DNS Server | `10.0.0.1` |
