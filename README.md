# security-monitoring-solution.github.io

## <ins> Network Overview </ins>
Your security assessment environment consists of four key machines, each with specific roles and IP addresses within the 192.168.113.0/24 subnet:
### <ins> Gateway (192.168.113.1/24) </ins>
Serves as the network gateway for all other machines
Configured with dual network adapters:
Bridge adapter: Provides direct access to the physical network
NAT adapter: Enables internet access for all internal machines while maintaining isolation
Acts as the central connection point, with confirmed connectivity to all three other machines
### <ins> Ubuntu Desktop (192.168.113.2/24) </ins>
Client machine for testing and monitoring
Used for conducting security assessments and analysis
Connected through the gateway for both internal and external access
### <ins> OpenVAS (192.168.113.3/24) </ins>
Vulnerability Assessment Scanner
Provides automated security scanning capabilities
Used to identify potential vulnerabilities in the network and systems
Generates detailed reports of security issues found
### <ins> Wazuh (192.168.113.4/24) </ins>
Wazuh is a security monitoring and the threat detection, identify, monitor, IT infrastructure.
Security Monitoring: Wazuh collects and analyze logs from different systems and application malicious activites, unauthorized access. 
Detection: Wazuh can detect potential attacks by analyzing system, network traffic, help organization.
File Intergrity Monitoring: Critical files and directories for unathorized changes.
Vulnerability Detction, Allowing organization, patch of vulnerability.
Provides real-time monitoring and threat detection

### <ins> Github Page </ins>
Github Pages is a free hosting service provided by Github that allows you to publish websites directly from your github repositories. 
Github pages is a static site hosting service that takes HTML, CSS, and JavaScript files directly from a repository on Github.
Websites are hosted as vaishu2000479.github.io or custom domains.
### <ins> Team Member Responsibilites </ins>
### Vaishnavi Bandiwar:
* Set up OpenVAS vulnerability scanner
* Configured the gateway with dual network adapters
## <ins>  </ins>
### Sami:
* Set up Ubuntu Desktop client
* Configured client-side testing tools (openvas)
## <ins> </ins> 
### Akshay Nagulkar:
* Prepared and delivered project presentation
* Coordinated demonstration of security assessment workflow
## <ins> </ins> 
### Vaishnavi Thorve:
* Set up Wazuh platform
* Created project documentation on GitHub
## <ins> </ins> 
## <ins> Network Configuration Details </ins>
The gateway machine serves as the cornerstone of this security assessment environment with its dual-adapter configuration:
Bridge Adapter: This provides the internal network with a direct connection to the physical network, enabling physical network resources to be accessible to the assessment environment.
NAT Adapter: The Network Address Translation adapter allows all internal machines (OpenVAS, Wazuh, Ubuntu Desktop) to access internet resources while maintaining network isolation for security purposes.
This configuration creates an isolated but fully functional security assessment lab where vulnerabilities can be detected (OpenVAS), security events can be monitored (Wazuh), and testing can be performed (Ubuntu Desktop), all while maintaining proper network segmentation through the gateway.
