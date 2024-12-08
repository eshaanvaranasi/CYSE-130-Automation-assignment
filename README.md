# CYSE-130-Automation-Assignment

Project Overview  
This project focuses on enhancing cybersecurity for a small business that currently relies on homemade tools and lacks proper security measures. The main goals include:  
1. Automating system monitoring using Python scripts.  
2. Securing sensitive data through encryption and access controls.  
3. Implementing network security and incident response mechanisms.  

The system addresses key client issues, including financial discrepancies, server security, and user authentication vulnerabilities.  

System Features  
- Data Encryption: Ensures encryption of sensitive data at rest and in transit using AES-256 and SSL/TLS.  
- Access Controls: Implements multi-factor authentication (MFA) and strict access restrictions to secure critical systems.  
- System Monitoring: Automates performance monitoring and vulnerability detection using refined Python scripts.  
- Incident Detection: Introduces logging, network traffic monitoring (Wireshark), and intrusion detection systems (IDS).  
- Network Security: Basic firewalls, SSH key-based authentication, and secure remote access.  
- Physical Security: Guidelines to lock down server access and restrict unauthorized physical entry.  

Installation  
Follow these steps to set up and run the project:  
1. Clone the Repository  
   ```
   git clone <repository_link>
   cd cybersecurity-system
   ```  
2. Install Dependencies:
   Ensure Python is installed (version 3.8+), and install necessary libraries:  
   ```
   pip install -r scripts/requirements.txt
   ```  
3. Set Up Monitoring Scripts:  
   Configure the scripts with the required directories and credentials:  
   - Edit `scripts/config.py` to specify server paths and log directories.  

4. Run Security Scripts:  
   - Monitor system logs:  
     ```
     python scripts/log_monitor.py
     ```  
   - Analyze network traffic:  
     ```
     python scripts/network_analysis.py
     ```  

5. Network Security Setup:  
   - Ensure firewalls are enabled and configured as outlined in `documentation/network_security.md`.  
   - Use SSH key-based authentication for remote connections.  

6. Encrypt Sensitive Data:  
   - Run encryption tools for file protection:  
     ```
     python scripts/encrypt_data.py --input <file_path> --output <encrypted_file>
     ```  

Usage  
1. Log Monitoring:  
   Monitors system logs for unauthorized access attempts and generates alerts for anomalies.  

2. Network Analysis:  
   Integrates with Wireshark and IDS tools (e.g., Snort) to analyze traffic and detect potential intrusions.  

3. Incident Detection:  
   Automatically logs security breaches and generates response steps based on severity.  

4. Data Security:  
   Secure sensitive files and emails using advanced encryption standards.  

5. Backup and Recovery:  
   Regular automated backups are stored securely and tested for recovery.  

Project Structure:
```
cybersecurity-system/  
├── README.md  
├── /scripts             # Python automation scripts  
│   ├── log_monitor.py  
│   ├── network_analysis.py  
│   ├── encrypt_data.py  
│   ├── config.py  
├── /diagrams            # UML diagrams (use-case and activity)  
├── /documentation       # System requirements, security protocols, and guidelines  
├── /results             # Analysis outputs and log summaries  
└── LICENSE  
```  

Team Members  
- Jay: Python Developer  
- Eshaan: Python Developer  
- Austin: Python Developer  
- Kehlani: Project Manager  
- Tony: UML Diagrams  
- Ali: Data Analyst  

Future Improvements  
- Implement advanced threat detection using AI-based anomaly detection.  
- Introduce enterprise-level security tools as the business grows.  
- Automate incident response workflows for faster mitigation.  
