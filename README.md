CYBERSECURITY LAB SETUP

Installing and Configuring Kali Linux Using Oracle VM VirtualBox

---

1. Project Overview

In this project, I set up a virtual cybersecurity laboratory using Oracle VM VirtualBox and Kali Linux.

The goal was to create an environment where I could learn and practice basic networking and cybersecurity concepts.

During this internship, I learned how to install and configure a Kali Linux virtual machine, create a virtual network using NAT Network, assign a manual IPv4 address, and test the network connection.

This practical work also helped me understand how virtualization works and gave me some hands-on experience with Linux and network configuration.

2. Project Objectives

The main objectives of this project were to:

- Install and run Kali Linux in Oracle VM VirtualBox.
- Create and configure a virtual NAT Network.
- Understand how virtual networks and network adapters work.
- Assign a manual IPv4 address.
- Learn about IP addresses, subnet prefixes, gateways, and DNS servers.
- Test network connectivity using the "ping" command.
- Check Internet access using Firefox.
- Gain practical experience with Linux and networking.
- Document the different steps of the setup.

3. Tools and Technologies

The following tools were used during this project:

Tool| Purpose
Oracle VM VirtualBox| Running the virtual machine
Kali Linux| Operating system used for cybersecurity practice
Windows| Main operating system of the laptop
Firefox| Testing Internet access
NAT Network| Connecting the virtual machine to external networks

4. Laptop Hardware Specifications

I used the following laptop for this project:

Component| Specifications
Host Operating System| Windows
Processor| 12th Gen Intel(R) Core(TM) i7-1265U
Installed RAM| 16 GB
Storage Capacity| 1 TB
Virtualization Software| Oracle VM VirtualBox 7.2.22
Additional Package| Oracle VM VirtualBox Extension Pack 7.2.22
Guest Operating System| Kali Linux

5. Virtual Machine Configuration

I configured the Kali Linux virtual machine using Oracle VM VirtualBox.

The network adapter was configured as follows:

Parameter| Configuration
Virtual Machine| Kali Linux
Network Adapter| Adapter 1
Adapter Type| Intel PRO/1000 MT Desktop (82540EM)
Network Mode| NAT Network
Network Name| natnetwork
Promiscuous Mode| Allow All
Cable Connected| Enabled

6. Network Configuration

For the network connection, I used the NAT Network feature available in VirtualBox.

The following IPv4 settings were used:

Parameter| Configuration
Network Name| natnetwork
Network Type| NAT Network
IPv4 Network| 10.0.0.0/24
DHCP| Enabled
Kali Linux IP Address| 10.0.0.3
Subnet Prefix| /24
Default Gateway| 10.0.0.1
DNS Server| 10.0.0.1
IPv6| Disabled

Understanding the Network Settings

During this exercise, I also learned what the different network settings mean:

- IP Address: Identifies a device on a network. In this case, it identifies my Kali Linux virtual machine.
- Subnet Prefix (/24): Defines the network portion of an IPv4 address.
- Default Gateway: Allows the virtual machine to communicate with networks outside its local network.
- DNS Server: Translates domain names into IP addresses so that websites can be accessed.
- NAT Network: Allows virtual machines to access external networks through the host computer's network connection.

7. Laboratory Setup and Implementation

7.1 Configuring the VirtualBox Network Adapter

The first thing I did was configure the network adapter of the Kali Linux virtual machine.

I enabled Adapter 1 and connected it to the NAT Network named "natnetwork".

The settings were:

- Attached to: NAT Network
- Name: natnetwork
- Adapter Type: Intel PRO/1000 MT Desktop (82540EM)
- Promiscuous Mode: Allow All
- Cable Connected: Enabled

Screenshot: VirtualBox Network Adapter Configuration

"VirtualBox Network Adapter" (screenshots/01-virtualbox-kali-network-adapter.jpg)

7.2 Starting Kali Linux

After configuring the network adapter, I started the Kali Linux virtual machine.

The system booted successfully and displayed the Kali Linux desktop. This confirmed that the virtual machine was running properly.

Screenshot: Kali Linux Desktop

"Kali Linux Desktop" (screenshots/02-kali-linux-desktop.jpg)

7.3 Configuring a Manual IPv4 Address

Next, I went to the network settings inside Kali Linux and entered the IPv4 configuration manually.

The values I used were:

- Address: 10.0.0.3
- Prefix: 24
- Gateway: 10.0.0.1
- DNS: 10.0.0.1

After entering these values, I applied the settings so that the virtual machine could use the configured network.

Screenshot: Manual IPv4 Configuration

"Kali IPv4 Configuration" (screenshots/03-kali-ipv4-manual-configuration.jpg)

7.4 Configuring the VirtualBox NAT Network

I also configured the NAT Network through the VirtualBox Network Manager.

The configuration included:

- Network Name: natnetwork
- IPv4 Prefix: 10.0.0.0/24
- DHCP: Enabled
- IPv6: Disabled

This created the virtual network that I used to connect Kali Linux and test its network connectivity.

Screenshot: VirtualBox NAT Network Configuration

"NAT Network Configuration" (screenshots/04-virtualbox-nat-network-configuration.jpg)

7.5 Testing Network Connectivity

Once the network configuration was completed, I opened the Kali Linux terminal and tested the connection using the following command:

ping 8.8.8.8

The terminal returned successful replies from the destination IP address.

This showed that Kali Linux was able to communicate with an external IP address during the test.

Screenshot: Ping Connectivity Test

"Ping Test" (screenshots/05-internet-connectivity-ping-test.jpg)

7.6 Checking Internet Access Using Firefox

After the ping test, I opened Firefox in Kali Linux and tried accessing Google.

The website loaded successfully, confirming that I could access web pages from the virtual machine.

Screenshot: Firefox Web Access

"Firefox Web Access" (screenshots/06-firefox-web-access-test.jpg)

8. Problems I Encountered and How I Solved Them

During the setup, I faced a few problems. Some of them took time to understand, but they also gave me an opportunity to improve my troubleshooting skills.

8.1 VirtualBox Network Tab Not Visible

Problem:

When I first installed Oracle VM VirtualBox, I noticed that the Network tab was not visible under the Tools section. This made it difficult to access the network settings I needed.

Solution:

I installed another version of VirtualBox. After that, I was able to access the network configuration options and continue with the setup.

8.2 Finding the Kali Linux Virtual Machine File

Problem:

I initially had difficulty finding the Kali Linux virtual machine file in File Explorer.

Solution:

I eventually used the Import option in VirtualBox to locate and import the Kali Linux virtual machine successfully.

I don't remember the exact steps I followed to locate the file, but I managed to complete the import process.

8.3 Understanding the Ping Command

Challenge:

Another difficulty I faced was understanding the networking concept behind the "ping" command.

The command worked, but I did not immediately understand what was happening in the background or how to interpret the results.

What I Learned:

I learned that the "ping" command is used to check whether a device or IP address can be reached over a network. I also started understanding how the replies help determine whether a connection is working.

9. Personal Challenges During the Internship

Apart from the technical difficulties, I also faced a personal challenge during the internship: my laptop was stolen.

This affected my progress because I had to ask my parents for additional money to buy another laptop so that I could continue working on the project.

Fortunately, I managed to get another laptop and continue with the practical work.

Because of this situation, I ended up submitting my project on the deadline day.

It was not an easy situation, but I learned that unexpected problems can happen, and sometimes you have to find a way to adapt and keep working.

10. My Previous Knowledge and Learning Experience

Before starting this practical exercise, I already had some experience with Ubuntu Linux.

However, I was not very familiar with networking concepts such as NAT Network, IPv4 addressing, gateways, and DNS configuration.

I learned most of these concepts through the explanations and guidance provided by the instructor during the internship.

Working on the laboratory setup helped me understand how these concepts are used in practice instead of only learning about them theoretically.

11. Skills and Knowledge I Gained

By completing this project, I gained practical experience in several areas, including:

- Setting up a virtual cybersecurity laboratory.
- Using Oracle VM VirtualBox.
- Running Kali Linux in a virtual machine.
- Configuring a NAT Network.
- Understanding IPv4 addresses and subnet prefixes.
- Assigning manual IP addresses.
- Understanding gateways and DNS servers.
- Using the "ping" command to test network connectivity.
- Checking Internet access using Firefox.
- Solving basic virtualization and networking problems.

One of the most useful things I learned was how to configure a Kali Linux virtual machine and establish a working network connection.

12. Self-Assessment

After completing this exercise, I feel confident that I can set up another Kali Linux virtual machine and configure its basic network settings on my own.

I now understand the main steps involved, from configuring the virtual machine and creating a NAT Network to assigning an IP address and testing the connection.

I still have more networking and cybersecurity concepts to learn, but this exercise gave me a good starting point and increased my interest in the field.

13. Security and Ethical Considerations

Throughout this project, the laboratory was used for educational purposes and authorized cybersecurity practice.

I also understand that activities such as network scanning and penetration testing should only be performed on systems that I own or have permission to test.

14. Conclusion

I successfully completed the setup of a virtual cybersecurity laboratory using Oracle VM VirtualBox and Kali Linux.

I configured the virtual machine to use a NAT Network, assigned it a manual IPv4 address, and tested the connection using the "ping" command and Firefox.

Both tests were successful. I was able to reach an external IP address and access websites from Kali Linux.

Although I faced some difficulties, including problems with VirtualBox configuration and the loss of my previous laptop, I managed to continue working and complete the project.

Overall, this internship helped me gain practical experience with virtualization, Linux, and basic networking. It also gave me more confidence in setting up a virtual laboratory independently and motivated me to continue learning about networking and cybersecurity.

15. Author Information

- Author: [Your Full Name]
- Project: Cybersecurity Lab Setup
- Host Operating System: Windows
- Virtualization Platform: Oracle VM VirtualBox 7.2.22
- Guest Operating System: Kali Linux
- Project Type: Practical Cybersecurity Laboratory

