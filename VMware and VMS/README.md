# README: Installation Guide for VMware and Virtual Machines

This README provides step-by-step instructions for installing VMware and setting up the necessary virtual machines (VMs) for a secure virtualized environment.

## Prerequisites

1. **System Requirements**:
   - Processor: Intel Core i5 or better
   - RAM: Minimum 16 GB (32 GB recommended)
   - Storage: At least 250 GB free space
   - Operating System: Windows 10/11 or Linux (64-bit)

2. **Software Downloads**:
   - VMware Workstation Pro: [https://www.vmware.com/products/workstation-pro.html](https://www.vmware.com/products/workstation-pro.html)
   - pfSense ISO: [https://www.pfsense.org/download/](https://www.pfsense.org/download/)
   - Security Onion ISO: [https://securityonion.net/](https://securityonion.net/)
   - Kali Linux ISO: [https://www.kali.org/downloads/](https://www.kali.org/downloads/)
   - Ubuntu Server ISO: [https://ubuntu.com/download/server](https://ubuntu.com/download/server)
   - Windows Server ISO: (Official licensing or trial from [Microsoft](https://www.microsoft.com))

---

## Installation Steps

### 1. Install VMware Workstation Pro

1. Download the VMware Workstation Pro installer from the official website.
2. Run the installer and follow the on-screen instructions:
   - Accept the license agreement.
   - Choose the default installation directory.
   - Complete the installation and restart your computer if prompted.
3. Launch VMware Workstation Pro and activate it using your license key (or use the trial version).

### 2. Create Virtual Machines

#### a) Create pfSense Firewall VM

1. Open VMware Workstation Pro and click **Create a New Virtual Machine**.
2. Select **Custom (advanced)** and click **Next**.
3. Choose the hardware compatibility (default recommended).
4. Select **Install an operating system later** and click **Next**.
5. Choose **Other** > **FreeBSD 64-bit** as the guest OS.
6. Assign:
   - Memory: 2 GB
   - Processors: 2
   - Network: 2 adapters (one for WAN, one for LAN)
   - Disk Size: 20 GB
7. Attach the pfSense ISO as the bootable image.
8. Power on the VM and follow the on-screen installation instructions.

#### b) Create Security Onion VM

1. Create a new VM and select **Linux** > **Ubuntu 64-bit** as the guest OS.
2. Assign:
   - Memory: 8 GB
   - Processors: 4
   - Disk Size: 50 GB
   - Network: Use a bridged adapter.
3. Attach the Security Onion ISO as the bootable image.
4. Install Security Onion following its setup wizard.

#### c) Create Kali Linux VM

1. Create a new VM and select **Linux** > **Debian 64-bit** as the guest OS.
2. Assign:
   - Memory: 4 GB
   - Processors: 2
   - Disk Size: 30 GB
   - Network: Use NAT or bridged adapter.
3. Attach the Kali Linux ISO as the bootable image.
4. Install Kali Linux using the guided setup.

#### d) Create Ubuntu Server VM

1. Create a new VM and select **Linux** > **Ubuntu 64-bit** as the guest OS.
2. Assign:
   - Memory: 4 GB
   - Processors: 2
   - Disk Size: 40 GB
   - Network: Use NAT.
3. Attach the Ubuntu Server ISO as the bootable image.
4. Follow the installation instructions to set up the server.

#### e) Create Windows Server VM

1. Create a new VM and select **Microsoft Windows** > **Windows Server 2019/2022** as the guest OS.
2. Assign:
   - Memory: 8 GB
   - Processors: 4
   - Disk Size: 80 GB
   - Network: Use bridged adapter.
3. Attach the Windows Server ISO as the bootable image.
4. Install Windows Server, configuring Active Directory and DNS as needed.

---

## Post-Installation Configuration

1. **Networking**:
   - Assign static IPs to all VMs.
   - Connect VMs via virtual network adapters as per your topology.
2. **Firewall Rules (pfSense)**:
   - Configure LAN/WAN interfaces.
   - Add rules to permit internal traffic and block unauthorized external connections.
3. **Monitoring Tools (Security Onion)**:
   - Configure Snort and Zeek for intrusion detection.
   - Set up dashboards for traffic analysis.
4. **Penetration Testing (Kali Linux)**:
   - Install and configure Metasploit and other testing tools.
5. **System Updates**:
   - Ensure all VMs are updated with the latest security patches.

---

## Troubleshooting

- **Performance Issues**: Allocate additional memory or disk space to critical VMs.
- **Network Connectivity**: Verify network adapter settings in VMware and ensure proper IP configurations.
- **Installation Errors**: Refer to official documentation for each software package.

---

This guide provides a structured approach to setting up VMware and the necessary virtual machines for building a secure and functional virtualized environment. For additional support, consult the official documentation or community forums.

