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

A NAT Network was selected because multiple virtual machines connected to the same NAT Network can communicate with one another while also having outbound network connectivity.

This will allow future attacker and target VMs to communicate within the lab

_______________________________________________________________________________________________________________________

Step 4. Import Kali Linux
The Kali Linux virtual machine was downloaded from the official Kali Linux website and imported into VirtualBox.

The VM network adapter was configured as follows:

Adapter 1
Attached to: NAT Network
Network:     NatNetwork
Adapter Type: Intel PRO/1000 MT Desktop
The VM was allocated:

RAM: 2048 MB

<img width="1619" height="971" alt="1-screenshot-kali-linux" src="https://github.com/user-attachments/assets/45212f9c-3101-4255-b20a-356968fbba49" />

________________________________________________________________________________________________________________________



Step 6. Create a Clean VM Snapshot
After completing the initial configuration, a VirtualBox snapshot was created.

Example snapshot name:

My First kali linux
The snapshot represents the clean baseline of the laboratory.

If a future exercise changes or damages the VM configuration, the machine can be restored to this baseline.

🔎 Lab Verification
✅ Test	🧾 Command	🎯 Expected Result
🌐 Check IP address	ip a	Correct Kali IP displayed
📡 Test gateway	ping 10.0.0.1	Successful replies
🌍 Test Internet connectivity	ping 10.0.0.1	Successful replies
🔎 Test DNS resolution	nslookup google.com	Domain resolves
🧰 Verify Nmap	nmap --version	Nmap version displayed
🔄 Verify snapshot	Restore snapshot and run ip a	Baseline configuration restored
Example Results
IP Address:
10.0.0.2/24

Gateway:
10.0.0.1

DNS:
10.0.0.1

🐞 Problems Encountered & Solutions
Documenting problems is an important part of the project.

## 🛠️Problem 1. Troubleshooting: Missing IPv4 Configuration Options in Kali Linux 

During the setup of my cybersecurity lab using Kali Linux on VMware Workstation Pro, I encountered an issue while trying to locate the IPv4 network configuration options.

The basic network menu displayed options such as:

- Ethernet
- Wired Disconnected
- VPN Connection

However, I could not immediately find the detailed IPv4 configuration fields, including:

- **Method:** Defines how the IP address is obtained, such as automatically through DHCP or manually.
- **Address:** The IP address assigned to the Kali Linux network interface.
- **Netmask:** Defines the network range associated with the IP configuration.
- **Gateway:** The network device used to reach destinations outside the local network.
- **DNS Servers:** Servers that translate domain names, such as `google.com`, into IP addresses.

Because these options were not visible in the basic network menu, I needed to investigate the existing network connection and locate the detailed configuration settings.

### 🔍 2. Troubleshooting Process

#### Step 1: Identify Saved Network Connections

I ran the following command to inspect the network connection profiles managed by NetworkManager.

```bash
nmcli connection show
```

**Purpose:** This command lists saved network connections, their types, and their associated network devices.

**What I checked:** I looked for the wired Ethernet connection and the device associated with it, such as `eth0`.

This helped me identify which connection profile needed further inspection.

#### Step 2: Inspect Network Interfaces and IP Addresses

Next, I ran:

```bash
ip a
```

**Purpose:** This command displays network interfaces, their current states, and assigned IP addresses.

The output showed:

- `lo` — the loopback interface, normally assigned `127.0.0.1`.
- `eth0` — the Ethernet network interface used by the Kali Linux virtual machine.

The `eth0` interface showed the IP address `10.0.0.2`.

This helped me identify the IP address assigned to the virtual machine's Ethernet interface.

#### Step 3: Open the NetworkManager Connection Editor

To access the detailed network settings, I executed:

```bash
nm-connection-editor
```

**Purpose:** This command opens the graphical NetworkManager connection editor, where available connection profiles can be inspected and configured.

In the editor, I selected the wired connection and opened its IPv4 settings.

This allowed me to access the detailed IPv4 configuration options that were not immediately available in the basic network menu.

<img width="1602" height="933" alt="3-screenshot-network-settings-2" src="https://github.com/user-attachments/assets/e77cadb8-63d0-4044-9cd0-be60a4d94fe2" />


### ✅ 3. Resolution

I successfully opened the NetworkManager connection editor and accessed the IPv4 settings for the wired connection.

I then reviewed and configured the required network settings for my lab environment.

After making the changes, I checked the network configuration and tested internet connectivity and DNS resolution to verify that the connection was working.

**Outcome:** I was able to access the detailed IPv4 configuration options and complete the required network configuration.

### 🧪 4. Verification Commands

After configuring the connection, I used the following commands to verify the network settings.

**Check the IPv4 address assigned to `eth0`:**

```bash
ip -4 addr show eth0
```

**Check the routing table and default gateway:**

```bash
ip route
```

**Test internet connectivity through a domain name:**

```bash
ping -c 4 google.com
```

**Test IP connectivity independently of DNS:**

```bash
ping -c 4 8.8.8.8
```

**Check DNS resolution:**

```bash
nslookup google.com
```

These commands helped verify the IP configuration, routing information, internet connectivity, and DNS resolution.

### 📚 5. Key Learnings

Through this troubleshooting process, I practised:

- Identifying saved network connection profiles using `nmcli`.
- Inspecting network interfaces and IP addresses using `ip a`.
- Understanding the role of the `eth0` network interface.
- Accessing advanced IPv4 settings through NetworkManager.
- Understanding the purpose of IP addresses, netmasks, gateways, and DNS servers.
- Verifying network connectivity using `ping`.
- Testing domain name resolution using `nslookup`.
- Following a systematic approach to Linux network troubleshooting.

### 🎯 6. Conclusion

This troubleshooting experience improved my understanding of network configuration in Kali Linux running on VMware Workstation Pro.

I learned how to investigate existing network connections, locate detailed IPv4 settings, and verify connectivity using command-line tools.

These skills provide a useful foundation for future cybersecurity lab activities, including network reconnaissance, port scanning, packet analysis, and authorized penetration testing.

______________________________________________________________________________________________________________________

Problem 2. VirtualBox VT-x / Virtualization Error
The VM initially failed to start because hardware virtualization was disabled in the system firmware/BIOS.
________________________________________________________________________________________________________________________

The issue was resolved by:

Restarting the computer.
Entering BIOS/UEFI settings.
Enabling Intel VT-x / hardware virtualization.
Saving the configuration.
Restarting the computer.
Starting the Kali VM again.
After enabling virtualization, the VM started successfully.

_______________________________________________________________________________________________________________________


## 📚 What I Have Learned

Through this cybersecurity lab setup, I gained practical experience with Kali Linux, VMware networking, and basic network troubleshooting.

### 1. Kali Linux and VMware
- Learned how Kali Linux runs inside a virtual machine using VMware Workstation Pro.
- Understood the basic role of a virtual machine in a cybersecurity lab.

### 2. Linux Networking Commands
- Used `ip a` to inspect network interfaces and IP addresses.
- Used `ip route` to check routing information and the default gateway.
- Used `nmcli connection show` to identify saved network connections.
- Used `nm-connection-editor` to access detailed network configuration settings.

### 3. IPv4 Network Configuration
- Learned the purpose of IPv4 addresses, netmasks, gateways, and DNS servers.
- Learned where to find IPv4 settings in NetworkManager.
- Practised investigating network configuration issues.

### 4. Internet Connectivity and DNS
- Used `ping -c 4 google.com` to test connectivity to a domain.
- Used `ping -c 4 10.0.0.1` to test IP connectivity.
- Used `nslookup google.com` to check DNS resolution.
- Learned that successful IP connectivity and successful DNS resolution are separate checks.

### 5. Troubleshooting Skills
- Learned to investigate network issues step by step.
- Practised checking network interfaces, connection profiles, and routing information.
- Learned to verify connectivity after changing network settings.

### 6. Cybersecurity Lab Documentation
- Practised documenting lab configurations and troubleshooting steps.
- Learned how to organize technical notes in Markdown.
- Improved my understanding of maintaining a GitHub portfolio for cybersecurity learning.

### 🎯 Key Takeaway

This lab helped me build a foundation in Linux networking, IPv4 configuration, DNS resolution, and network troubleshooting. These skills will support my future learning in network reconnaissance, vulnerability assessment, and authorized penetration testing.
______________________________________________________________________________________________________________________

🔐 Security & Ethical Use
This laboratory is intended strictly for education purposes only.

______________________________________________________________________________________________________________________


