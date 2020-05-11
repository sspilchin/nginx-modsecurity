**Nginx version 1.18 with WAF (Web Application Firewall)**

-  ModSecurity version 2.9.3 
-  OWASP CRS ( ModSecurity Core Rule Set)

The Nginx module is contained within the Apache archive package.
Usually you must first compile ModSecurity with the --enable-standalone-module flag and then compile the Nginx code to use it.

If you can’t afford a commercial web application firewall, this would be an excellent choice to go for it.

To provide generic web applications protection, the Core Rules use the following techniques:

- HTTP Protection – detecting violations of the HTTP protocol and a locally defined usage policy
- Real-time Blacklist Lookups – utilizes 3rd Party IP Reputation
- Web-based Malware Detection – identifies malicious web content by check against the Google Safe Browsing API.
- HTTP Denial of Service Protections – defense against HTTP Flooding and Slow HTTP DoS Attacks.
- Common Web Attacks Protection – detecting common web application security attack
- Automation Detection – Detecting bots, crawlers, scanners, and another malicious surface activity
- Integration with AV Scanning for File Uploads – identifies malicious files uploaded through the web application.
- Tracking Sensitive Data – Tracks Credit Card usage and blocks leakages.
- Trojan Protection – Detecting access to Trojans horses.
- Identification of Application Defects – alerts on application misconfigurations.
- Error Detection and Hiding – Disguising error messages sent by the server.

**OWASP CRS ( ModSecurity Core Rule Set)**

The OWASP ModSecurity Core Rule Set (CRS) is a set of generic attack detection rules for use with ModSecurity or compatible web application firewalls. The CRS aims to protect web applications from a wide range of attacks, including the OWASP Top Ten, with a minimum of false alerts.
