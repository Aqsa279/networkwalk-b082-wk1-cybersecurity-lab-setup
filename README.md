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

________________________________________________________________________________________________________________________

🪜 Lab Setup Procedure
Step 1. Install 7-Zip
7-Zip was installed to extract the Kali Linux virtual-machine package, which may be distributed as a .7z archive.

Tool: 7-Zip

Step 2. Install VirtualBox
VirtualBox has installed 


🔐 Cybersecurity Lab Environment Setup
Building an isolated virtual lab for penetration testing and ethical hacking practice

           

📌 Project Overview
This project focuses on setting up a virtual cybersecurity and penetration-testing laboratory using VirtualBox and Kali Linux.

The purpose of the lab is to create a controlled environment where cybersecurity tools, network scanning, reconnaissance, vulnerability assessment, and other security-testing activities can be performed safely and repeatedly.

The lab is configured on a private virtual network so that additional machines can be added later and used as targets for authorized security testing.

🎯 Objectives
The main objectives of this project are to:

Install and configure VirtualBox.
Install/import Kali Linux as a virtual machine.
Create a private NAT Network for the cybersecurity lab.
Configure network connectivity for Kali Linux.
Assign a consistent IP address to the Kali VM.
Verify network connectivity and DNS resolution.
Take a clean VM snapshot for recovery.
Document the complete setup process.
Prepare the environment for future cybersecurity projects.
🛡️ Purpose of the Lab
The lab provides an isolated and controlled environment for cybersecurity learning and authorized security testing.

It can be used for activities such as:

Network reconnaissance
Port scanning
Vulnerability assessment
Packet analysis
Web security testing
Exploitation practice
Security-tool experimentation
⚠️ Important: This laboratory must only be used for systems that you own or have explicit permission to test. Do not use the lab or its tools to attack unauthorized systems.

🏗️ Lab Architecture


Additional target machines can be added to the same virtual network in future projects.

⚙️ Lab Configuration
🧩 Component	⚙️ Configuration
🖥️ Host OS	Windows 10
🧠 Host RAM	8 GB
⚡ Processor	Intel Core i7
🧰 Hypervisor	VirtualBox 7.2
🐉 Security OS	Kali Linux 2026.2
🧠 Kali RAM	2048 MB
🌐 Virtual Network	NAT Network
📡 Network Address	10.0.0.0/24
🐧 Kali IP Address	10.0.0.2/24
🚪 Default Gateway	10.0.0.1
🌍 DNS Server	8.8.8.8
🔮 Future VM Range	10.0.0.3–10.0.0.99
🪜 Lab Setup Procedure
Step 1. Install 7-Zip
7-Zip was installed to extract the Kali Linux virtual-machine package, which may be distributed as a .7z archive.

Tool: 7-Zip

Step 2. Install VirtualBox
VirtualBox was installed as the hypervisor.

Step 3. Create the NAT Network
NAT Network was created in VirtualBox.

Configuration: Network Name: NatNetwork IPv4 Prefix: 10.0.0.0/24 DHCP: Enabled IPv6: Disabled

<img width="1919" height="1003" alt="2-screenshot-network-settings-1" src="https://github.com/user-attachments/assets/fbd979f6-4965-4fa1-9453-b9dbcb791ccd" />


