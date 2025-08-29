# Phishing-Campaign-Simulation-and-Detection-Lab


### 🎯 Goal

This project documents a hands-on cybersecurity exercise to simulate a full-spectrum phishing attack and analyze the resulting network and host-based evidence. The primary objective was to gain practical experience in both offensive (threat simulation) and defensive (detection & analysis) disciplines, which are critical for a career in Security Operations.

### ⚙️ Tools & Setup

* **Platform:** Oracle VirtualBox
* **Attacker VM:** Ubuntu Linux
* **Victim VM:** Windows
* **Offensive Tools:** GoPhish
* **Defensive Tools:** Wireshark, Windows Event Viewer

### 🛠️ What I Did

This lab was executed in two distinct phases:

1.  **Threat Simulation (Red Team):**
    * Configured and ran a GoPhish server on the Ubuntu VM.
    * Crafted a convincing phishing email and a simple, custom landing page to align the social engineering narrative.
    * Launched a targeted phishing campaign to my Windows VM to generate a controlled security event.

2.  **Detection & Analysis (Blue Team):**
    * Utilized **Wireshark** to perform a network packet capture of the attack traffic. Analyzed the HTTP stream to successfully identify and extract clear-text credentials, demonstrating the vulnerability of unencrypted protocols.
    * Examined the **Windows Event Viewer** to identify and analyze host-based logs associated with the simulated attack activity.

### 🧠 Why It Matters

This exercise provides a comprehensive, end-to-end understanding of an email-based attack from both sides of the cyber kill chain. Key skills demonstrated include:

* **Incident Investigation:** The ability to methodically trace an attack's footprint across multiple data sources (network traffic and host logs).
* **Threat Detection:** Practical experience configuring a phishing tool and analyzing its output for signs of a successful attack.
* **Packet Analysis:** Hands-on proficiency with Wireshark to inspect and interpret network traffic for sensitive information.
* **Foundational Knowledge:** A strong grasp of core cybersecurity concepts, including social engineering, the difference between HTTP and HTTPS, and the role of host-based vs. network-based logging.

### 💡 Future Work

To expand on this lab, I plan to integrate a SIEM like **Splunk** to ingest logs from both the GoPhish server and the Windows VM, allowing for automated detection rules and a more scalable incident response workflow.
