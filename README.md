# Custom Syslog Generator 📡

A Python Network Security utility built to inject custom, spoofed, or standardized Syslog packets into a SIEM (Security Information and Event Management) environment. Designed to help SOC Analysts test and validate alerting rules, dashboards, and automated playbooks.

**Features:**
* Constructs properly formatted RFC 3164 Syslog headers by calculating strict `<PRIVAL>` values from Facility and Severity inputs.
* Employs Python's native `socket` library to rapidly transmit stateless UDP Datagrams over Port 514.
* Features quick-select presets simulating common network anomalies, including Cisco IOS interface failures, ASA firewall drops, and Linux SSH brute-force attempts.
* Dynamically stamps packets with the host operating system's current timestamp and machine node name.

*Built as Day 15 of a 30-Day Network Engineering & Security portfolio streak.*
