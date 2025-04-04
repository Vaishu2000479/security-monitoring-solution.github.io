# security-monitoring-solution.github.io
# Network Overview
Your security assessment environment consists of four key machines, each with specific roles and IP addresses within the 192.168.113.0/24 subnet:
# Gateway (192.168.113.1)
Serves as the network gateway for all other machines
Configured with dual network adapters:
Bridge adapter: Provides direct access to the physical network
NAT adapter: Enables internet access for all internal machines while maintaining isolation
Acts as the central connection point, with confirmed connectivity to all three other machines
# Ubuntu Desktop (192.168.113.2)
Client machine for testing and monitoring
Used for conducting security assessments and analysis
Connected through the gateway for both internal and external access
# OpenVAS (192.168.113.3)
Vulnerability Assessment Scanner
Provides automated security scanning capabilities
Used to identify potential vulnerabilities in the network and systems
Generates detailed reports of security issues found
# Wazuh (192.168.113.5)
Security Information and Event Management (SIEM) platform
Provides real-time monitoring and threat detection
Handles log analysis and security event correlation
Offers intrusion detection capabilities
# Team Member Responsibilities
Vaishnavi:
Set up OpenVAS vulnerability scanner
Configured the gateway with dual network adapters
Sami:
Set up Ubuntu Desktop client
Configured client-side testing tools
Akshay:
Prepared and delivered project presentation
Coordinated demonstration of security assessment workflow
Vaishnavi:
Set up Wazuh SIEM platform
Created project documentation on GitHub
# Network Configuration Details
The gateway machine serves as the cornerstone of this security assessment environment with its dual-adapter configuration:
Bridge Adapter: This provides the internal network with a direct connection to the physical network, enabling physical network resources to be accessible to the assessment environment.
NAT Adapter: The Network Address Translation adapter allows all internal machines (OpenVAS, Wazuh, Ubuntu Desktop) to access internet resources while maintaining network isolation for security purposes.
This configuration creates an isolated but fully functional security assessment lab where vulnerabilities can be detected (OpenVAS), security events can be monitored (Wazuh), and testing can be performed (Ubuntu Desktop), all while maintaining proper network segmentation through the gateway.
