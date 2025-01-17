# Thesis
Thesis of bachelor degree  
# Security Assessment and Hardening of Network Devices

This repository contains the project files, configurations, and documentation for the thesis **"Security Assessment and Hardening of Network Devices."**

## **Overview**
This project focuses on securing network devices by implementing and assessing various security measures. It utilizes a virtual environment comprising the following components:

- **VMware**
- **pfSense Firewall**
- **Windows Client VM**
- **Kali Linux (Attacker VM)**
- **Ubuntu Server VM**
- **Security Onion VM**
- **Windows Server VM**
- **Splunk** (for data forwarding and analysis)

## **Project Features**
1. **Firewall Configuration:** Securing networks using pfSense.
2. **Intrusion Detection/Prevention:** Using Security Onion for monitoring and alerting.
3. **Endpoint Security:** Hardening Windows and Ubuntu servers.
4. **Centralized Logging:** Configuring Splunk to collect and analyze system logs.
5. **Vulnerability Assessment:** Using Kali Linux to identify weaknesses.

## **Structure of the Repository**
- `configs/`: Configuration files for pfSense, Security Onion, and other VMs.
- `screenshots/`: Key screenshots illustrating the configurations and results.
- `scripts/`: Scripts used for automation or configuration.
- `documentation/`:
  - `thesis_final.pdf`: Final version of the thesis document.
  - `config_descriptions.md`: Detailed descriptions of configurations.
- `videos/`: Demonstration videos of the project.(If possible)

## **Setup Instructions**
### **Prerequisites**
1. VMware installed with support for multiple VMs.
2. Access to the following VMDK/ISO files:
   - pfSense
   - Ubuntu Server
   - Security Onion
   - Windows Server
   - Kali Linux
3. Basic networking knowledge.

## **Usage**
1. Install VMware Workstation. Start all VMs in the VMware environment.
2. Use pfSense to manage network traffic and security policies.
3. Monitor network activity using Security Onion.
4. Perform security assessments with Kali Linux.
5. Collect logs and analyze them using Splunk.

## **Results**
The project highlights effective methods for securing network devices and demonstrates:
- Reduced vulnerability to common attacks.
- Improved network visibility and monitoring.
- Centralized log management and analysis.

## **Challenges and Lessons Learned**
1. Configuring VMs with limited resources.
2. Debugging network connectivity issues.
3. Learning and implementing advanced Splunk queries.

## **Contact**
For questions or contributions, please reach out:
- **Name:** Alijon Nazarov
- **Email:** anazaro1@stu.vistula.edu.pl
- **GitHub:** (https://github.com/ALNA0770)

---
Thank you for exploring this project! Feel free to suggest improvements or report issues in the repository.
