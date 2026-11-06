
# CYBERSECURITY LAB SETUP
### Practical Installation and Network Configuration of Kali Linux Using Oracle VM VirtualBox

---

## 1. Project Overview

This project focuses on setting up a virtual cybersecurity laboratory using Oracle VM VirtualBox and Kali Linux.

The main purpose of this practical exercise was to create a virtual environment where I could learn and practice basic networking concepts and cybersecurity techniques.

During this internship, I learned how to configure a Kali Linux virtual machine, establish a virtual network using NAT Network, assign a manual IPv4 address, and test network connectivity.

This project also helped me develop practical knowledge of virtualization, Linux environments, and basic network configuration.

## 2. Project Objectives

The main objectives of this project were:

- Set up and run Kali Linux in Oracle VM VirtualBox.
- Configure a virtual NAT Network.
- Understand virtual networking and network adapter configuration.
- Configure a manual IPv4 address.
- Understand IP addresses, subnet prefixes, gateways, and DNS servers.
- Test network connectivity using the ping command.
- Verify Internet access using Firefox.
- Gain practical knowledge of Linux and networking.
- Document the laboratory setup with screenshots.

## 3. Tools and Technologies

The following tools and technologies were used:

| Tool | Purpose |
|---|---|
| Oracle VM VirtualBox | Virtualization software |
| Kali Linux | Guest operating system for cybersecurity practice |
| Windows | Host operating system |
| Firefox | Web browser for Internet connectivity testing |
| NAT Network | Virtual networking configuration |

## 4. Laptop Hardware Specifications

The following hardware was used as the host system for this cybersecurity laboratory:

| Component | Specifications |
|---|---|
| Host Operating System | Windows |
| Processor | 12th Gen Intel(R) Core(TM) i7-1265U |
| Installed RAM | 16 GB |
| Storage Capacity | 1 TB |
| Virtualization Software | Oracle VM VirtualBox 7.2.22 |
| Additional Package | Oracle VM VirtualBox Extension Pack 7.2.22 |
| Guest Operating System | Kali Linux |

## 5. Virtual Machine Configuration

The Kali Linux virtual machine was configured using Oracle VM VirtualBox.

The following configuration was used:

| Parameter | Configuration |
|---|---|
| Virtual Machine | Kali Linux |
| Network Adapter | Adapter 1 |
| Adapter Type | Intel PRO/1000 MT Desktop (82540EM) |
| Network Mode | NAT Network |
| Network Name | natnetwork |


## 6. Network Configuration

The virtual network was configured using VirtualBox NAT Network.

The following IPv4 configuration was used:

| Parameter | Configuration |
|---|---|
| Network Name | natnetwork |
| Network Type | NAT Network |
| IPv4 Network | 10.0.0.0/24 |
| DHCP | Enabled |
| Kali Linux IP Address | 10.0.0.3 |
| Subnet Prefix | /24 |
| Default Gateway | 10.0.0.1 |
| DNS Server | 10.0.0.1 |
| IPv6 | Disabled |

## 7. Laboratory Setup and Implementation

### 7.1 VirtualBox Network Adapter Configuration

The first step involved configuring the network adapter of the Kali Linux virtual machine.

Adapter 1 was enabled and connected to the NAT Network named `natnetwork`.

The adapter was configured with the following settings:

- Attached to: NAT Network
- Name: natnetwork
- Adapter Type: Intel PRO/1000 MT Desktop (82540EM)

### 7.2 Starting Kali Linux

After configuring the virtual network adapter, the Kali Linux virtual machine was started successfully.

The Kali Linux desktop environment was displayed, confirming that the virtual machine was running.

### 7.3 Manual IPv4 Configuration

The network settings inside Kali Linux were configured manually.

The following values were entered:

- Address: 10.0.0.3
- Prefix: 24
- Gateway: 10.0.0.1
- DNS: 10.0.0.1

These settings allowed the Kali Linux virtual machine to communicate through the configured virtual network.


### 7.4 Configuring the VirtualBox NAT Network

The VirtualBox NAT Network manager was configured with the following settings:

- Network Name: natnetwork
- IPv4 Prefix: 10.0.0.0/24
- DHCP: Enabled
- IPv6: Disabled

This network configuration provided the virtual machine with a network environment for connectivity testing.


### 7.5 Testing Network Connectivity

After completing the network configuration, a connectivity test was performed using the Linux terminal.

The following command was executed:

```bash
ping 8.8.8.8
```

The terminal displayed successful replies from the destination IP address.

This confirmed that the Kali Linux virtual machine could communicate with the external IP address during the test.



### 7.6 Testing Internet Access Using Firefox

Finally, Firefox was opened inside Kali Linux.

Google was accessed successfully, demonstrating that web access was available from the virtual machine.


## 8. Problems Encountered and Solutions

During the laboratory setup, I encountered some difficulties that helped me develop my troubleshooting skills.

### 8.1 VirtualBox Network Tab Not Visible

**Problem:**

During the initial installation of Oracle VM VirtualBox, I encountered a version in which the Network tab was not visible under the Tools section.

**Solution:**

I installed another version of VirtualBox, which allowed me to access the network configuration options needed for the laboratory setup.

### 8.2 Locating the Kali Linux Virtual Machine

**Problem:**

Initially, I went to File Explorer to locate the Kali Linux virtual machine files, but I could not find the file I needed.

**Solution:**

I eventually used the Import option in Oracle VM VirtualBox and was able to locate and import the Kali Linux virtual machine successfully.



### 8.3 Understanding the Ping Command

**Challenge:**

One of the most challenging parts of this practical exercise was understanding the networking concept behind the ping command.

Although the connectivity test worked immediately, understanding what the command does and how to interpret its results required more attention.

**Learning Outcome:**

I gained a better understanding of how the ping command can be used to test connectivity between devices and external IP addresses.

## 9. Personal Challenges During the Internship

One of the biggest difficulties I faced during this internship was that my laptop was stolen.

This situation affected my progress because I had to ask my parents for additional money to purchase another laptop so that I could continue working on the project.

Despite this unexpected situation, I managed to obtain another laptop and continue with the practical work.

As a result, I submitted my project on the deadline day.

This experience taught me the importance of perseverance, determination, and adapting to unexpected challenges.

## 10. Previous Knowledge and Learning Experience

Before starting this practical exercise, I was already familiar with Ubuntu Linux.

However, I did not have a strong understanding of networking concepts such as NAT Network, IPv4 addressing, gateways, and DNS configuration.

During the internship, I learned these concepts through explanations and guidance from the instructor.

The practical exercise helped me connect theoretical networking concepts with their actual implementation in a virtual laboratory.

## 11. Skills and Knowledge Acquired

Through this laboratory exercise, I gained practical knowledge and experience in:

- Setting up a virtual cybersecurity laboratory.
- Using Oracle VM VirtualBox.
- Running Kali Linux in a virtual machine.
- Configuring VirtualBox NAT Network.
- Understanding IPv4 addressing and subnet prefixes.
- Configuring manual IP addresses.
- Understanding gateways and DNS servers.
- Testing network connectivity using the ping command.
- Verifying Internet access using Firefox.
- Troubleshooting basic virtualization and networking problems.

One of the most important things I learned was how to independently configure a Kali Linux virtual laboratory and establish network connectivity.

## 12. Self-Assessment

After completing this practical exercise, I feel very confident about setting up another Kali Linux virtual laboratory independently.

I now have a better understanding of the steps involved in configuring a virtual machine, establishing a NAT Network, assigning network settings, and testing connectivity.

This experience has also increased my interest in learning more about networking and cybersecurity.


## 14. Conclusion

The cybersecurity laboratory setup was successfully completed using Oracle VM VirtualBox and Kali Linux.

The virtual machine was connected to a NAT Network, configured with a manual IPv4 address, and tested using the ping command and Firefox browser.

The successful connectivity tests demonstrated that the virtual machine could communicate with an external IP address and access web resources.

Although I encountered some difficulties during the process, including VirtualBox configuration issues and personal challenges, I successfully completed the practical exercise.

This internship provided me with a valuable foundation in virtualization, Linux environments, network configuration, and basic cybersecurity laboratory setup.

It also increased my confidence in independently creating and configuring a virtual cybersecurity laboratory.

## 15. Author Information

- **Author:**Ishatse Fleury
- **Project:** Cybersecurity Lab Setup
- **Host Operating System:** Windows
- **Virtualization Platform:** Oracle VM VirtualBox 7.2.22
- **Guest Operating System:** Kali Linux
- **Project Type:** Practical Cybersecurity Laboratory

