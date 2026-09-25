# Methodology and Attack Sequence

## 1. Pre-Engagement and Scope

The engagement began with an agreed testing scope covering authorized MegaQuagga systems and services.

## 2. Reconnaissance

I identified reachable hosts, exposed services, WordPress components, directories, users, and plugins.

Tools used:

- Nmap
- Gobuster
- WPScan

## 3. Vulnerability Discovery

I performed deeper scanning and enumeration to identify known vulnerabilities and configuration weaknesses.

Tools used:

- Nmap scripting
- Nuclei
- Nikto
- WPScan

## 4. WordPress Exploitation

A vulnerable WordPress component was identified and validated.

The exploitation sequence included:

- Preparing a test payload
- Hosting the payload for retrieval
- Triggering the vulnerable functionality
- Establishing a reverse shell
- Confirming shell access

Tools used:

- WPScan
- cURL
- Metasploit
- Meterpreter
- Netcat

## 5. Credential Attack

A separate WordPress target was tested for weak authentication controls.

The sequence included:

- Enumerating valid WordPress usernames
- Performing credential brute-force testing
- Successfully authenticating to an administrative account

Tools used:

- WPScan
- Hydra

## 6. Privilege Escalation

After gaining host access, I enumerated SUID-enabled binaries and identified a privilege-escalation opportunity.

The sequence included:

- Enumerating SUID binaries
- Reviewing potential escalation paths
- Testing elevated access
- Confirming root-level access

Tools used:

- find
- sudo
- searchsploit
- perl
- gcc

## 7. Post-Exploitation

After access was established, I evaluated the potential impact of the compromise.

Activities included:

- Reviewing configuration files
- Gathering credentials
- Reviewing logs and command history
- Identifying potential persistence opportunities
- Mapping additional internal systems
- Identifying potential lateral movement opportunities
- Demonstrating impact through access to the WordPress application

## 8. Reporting and Remediation

The final phase documented the findings, prioritized the identified weaknesses, and provided remediation guidance.

Recommendations included:

- WordPress patching
- Stronger passwords
- Multi-factor authentication
- SUID permission reviews
- Network segmentation
- Least privilege
- Improved logging and monitoring
