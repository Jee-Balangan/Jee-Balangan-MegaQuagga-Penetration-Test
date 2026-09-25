# Methodology and Tools

## Assessment Methodology

The penetration test followed a structured workflow that moved from reconnaissance through exploitation and post-exploitation.

## 1. Reconnaissance

I began by identifying reachable systems, open ports, exposed services, and web application components.

Tools used:

- Nmap
- Gobuster
- WPScan

This phase helped identify WordPress services, directories, users, plugins, and other potential attack paths.

## 2. Vulnerability Scanning

I performed additional scanning to identify known vulnerabilities and configuration weaknesses.

Tools used:

- Nuclei
- Nikto
- Nmap scripting

The goal was to identify issues that could be validated during the exploitation phase.

## 3. Exploitation

The assessment validated several identified weaknesses in the authorized environment.

Testing included:

- WordPress exploitation
- Credential brute-force testing
- Reverse shell execution
- Privilege escalation testing

Tools used:

- Hydra
- Metasploit
- Meterpreter
- Netcat
- cURL

## 4. Privilege Escalation

I reviewed the Linux host for privileged binaries and other escalation opportunities.

Tools and techniques included:

- SUID binary enumeration
- `find`
- `sudo`
- `searchsploit`
- `perl`
- `gcc`

The assessment confirmed escalation to root-level access.

## 5. Post-Exploitation

After access was obtained, I evaluated the potential impact of the compromise.

Activities included:

- Reviewing configuration files
- Reviewing logs and command history
- Identifying potential persistence opportunities
- Mapping additional systems
- Identifying potential lateral movement paths

## 6. Reporting and Remediation

The final phase focused on documenting the findings and providing remediation recommendations.

Recommendations addressed:

- WordPress patching
- Password security
- Multi-factor authentication
- SUID permissions
- Network segmentation
- Least privilege
- Logging and monitoring

## Tools Used

- Nmap
- Gobuster
- WPScan
- Hydra
- Metasploit
- Meterpreter
- Nuclei
- Nikto
- Netcat
- cURL
- searchsploit
- gcc
- perl
- find
- sudo
