# Wireshark-Packet-Analysis-Learning-Journey-Submission-3MTT-July-Showcase-2
******Project Titl****e**: Decoding Cyber Threats with Wireshark: A Beginner’s Deep Dive  
****Name****: Tracy Nworie  
**Fellow ID**: FE/24/686089367  
****Cohort****: 3 (Cybersecurity Track)  
***Tool Used**: Wireshark
## 🧠 Project Overview
This project is part of the **3MTT Knowledge Showcase (July 2025 Edition)**, submitted under the **Learning Journey** category.  
It demonstrates the use of **Wireshark**, a packet capturing and analysis tool, to examine potentially malicious network activity and simulate basic threat detection.
##  Project Structure
 b wireshark-packet-analysis
- malicious_download.pcapng # Sample capture file
- incident_report.pdf # Summary report of findings
-walkthrough_video.mp4 # 3-minute demo video
-screenshots/ # Screenshots of Wireshark filters and findings
- README.md # Project documentation
##  Analysis Summary
- **Scenario**: A suspected malicious file was downloaded from a fake software site.
 - **Traffic Observed**:
 - DNS resolution to suspicious domain
 - HTTP GET request for an executable file
- Repeated outbound connections to foreign IP addresses
- **Detection**:
 - Used Wireshark filters:
- `http.request`
 - `dns.qry.name contains ".exe"`
 - `ip.addr == suspicious_IP`
- **Outcome**: Confirmed signs of **malicious file download** and **data exfiltration attempt**.
## Incident Response Report
View Full Report [here](https://docs.google.com/document/d/1M0Qp5PG571Mds8utdzMlziWJVFrKQFyqYz8rn3Yo9Ys/edit?usp=sharing) incident_report.

Contents:
- Timeline of network activity
- IOC (Indicators of Compromise)
- Packet details with screenshots
- Remediation suggestions
## 📷 Sample Screenshots
<p align="center">
<img src="screenshots/http_get_request.png" width="500"/>
<img width="1439" height="556" alt="image" src="https://github.com/user-attachments/assets/d19f80d5-bf4f-48f2-a968-1fff9c0acfc4" />
<br>
 <em>Fig 1: HTTP GET Request for suspicious .exe file</em>
<img width="976" height="500" alt="image" src="https://github.com/user-attachments/assets/cdb6f09c-b1e7-42de-b418-0a59a36c1bb3" />
</p>
<p align="center">
<img src="screenshots/dns_query.png" width="500"/>
<img width="1573" height="517" alt="image" src="https://github.com/user-attachments/assets/17c6a219-2117-4c59-946e-0d432ba2efa9" />
<br>
 <em>Fig 2: DNS query to suspicious domain</em>
<img width="928" height="470" alt="image" src="https://github.com/user-attachments/assets/6feaefc3-b342-4fad-8335-0ca0969b5961" />
</p>
## 🎥 Video Demonstration
A 3-minute walkthrough where I:
1. Load the capture file
2. Apply filters to analyze traffic
3. Explain findings and the learning process

📺 Watch Video [Here](#)

## 🙌 Acknowledgments
Special thanks to:
- **3MTT Nigeria** for the opportunity and platform
- Honourable Minister **Dr. Bosun Tijani** for championing digital transformation
- The supportive community of **3MTT Fellows**
- **Darey.io** community learning path for your comprehensive training modules 

## 📲 Connect
🧕🏽 Tracy Nworie  
🔗 LinkedIn: [here](https://www.linkedin.com/in/tracy-nworie-8abb806a/?lipi=urn%3Ali%3Apage%3Ad_flagship3_profile_view_base%3BscV3Gz9%2FScSbBxg8jaOBSg%3D%3D)  
📧 Email: [tracycelestina07@gmail.com]  

>  _“Every packet tells a story. Learning to read that story is the first step toward cyber resilience.”_











