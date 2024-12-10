# Cybersecurity Framework NIST  

> Please visit this [link](https://www.coursera.org/learn/networks-and-network-security?specialization=google-cybersecurity) for further information.

## Scenario 

You are a cybersecurity analyst working for a multimedia company that offers web design services, graphic design, and social media marketing solutions to small businesses. Your organization recently experienced a DDoS attack, which compromised the internal network for two hours until it was resolved.
During the attack, your organization’s network services suddenly stopped responding due to an incoming flood of ICMP packets. Normal internal network traffic could not access any network resources. The incident management team responded by blocking incoming ICMP packets, stopping all non-critical network services offline, and restoring critical network services. 
The company’s cybersecurity team then investigated the security event. They found that a malicious actor had sent a flood of ICMP pings into the company’s network through an unconfigured firewall. This vulnerability allowed the malicious attacker to overwhelm the company’s network through a distributed denial of service (DDoS) attack. 
To address this security event, the network security team implemented: 
- A new firewall rule to limit the rate of incoming ICMP packets
- Source IP address verification on the firewall to check for spoofed IP addresses on incoming ICMP packets
- Network monitoring software to detect abnormal traffic patterns
- An IDS/IPS system to filter out some ICMP traffic based on suspicious characteristics
As a cybersecurity analyst, you are tasked with using this security event to create a plan to improve your company’s network security, following the National Institute of Standards and Technology (NIST) Cybersecurity Framework (CSF). You will use the CSF to help you navigate through the different steps of analyzing this cybersecurity incident and integrate your analysis into a general security strategy:

1. Identify security risks through regular audits of internal networks, systems, devices, and access privileges to identify potential gaps in security. 
2. Protect internal assets through the implementation of policies, procedures, training and tools that help mitigate cybersecurity threats. 
3. Detect potential security incidents and improve monitoring capabilities to increase the speed and efficiency of detections. 
4. Respond to contain, neutralize, and analyze security incidents; implement improvements to the security process. 
5. Recover affected systems to normal operation and restore systems data and/or assets that have been affected by an incident.

## Respond

### Summary

ICMP/ping flood attack is possible due to multiple compromised systems sending a huge volume of ICMP echo requests to the target. In this case, ICMP/ping flood causes network services to become unresponsive or stop working. Then, the organization decided to block the flood attack and stop all non-critical network services to overcome the disruptions caused by denial of services (DDos) through incoming ICMP/Ping flood packets.

### NIST CSF 

1	Identify:
- Technology/Asset: Which systems and devices were affected?
- Process/Business Environment: Which business processes were impacted by the attack?
- People: Who needs access to the affected systems?

 Response: The attacker targeted the company with an ICMP flood attack, disrupting the internal network and preventing staff from performing operational tasks. To restore functionality, the internal network must be repaired promptly.
 
2	Protect: Implement safeguards:
- Access Controls: Who needs access to the affected items? How can access by untrusted sources be restricted?
- Awareness/Training: Who should be informed about this attack, and how can future attacks be prevented?
- Data Security: Are there any compromised data assets that need enhanced security?
- Information Protection and Procedures: Should any policies or procedures be updated to safeguard data?
- Maintenance: Should any affected hardware, OS, or software be updated?
- Protective Technology: What protective technologies, like firewalls or intrusion prevention systems (IPS), should be implemented?

 Response: The cybersecurity team should be immediately alerted during an attack. Since staff rely on the internal network, implementing a firewall rule to limit incoming ICMP packets and regularly updating it to address emerging threats is essential. Additionally, the team should ensure that devices, operating systems, and software are updated and monitored. Introducing an IDS/IPS system would help identify and block suspicious ICMP traffic patterns effectively.
 
3	Detect: Identify threats and attacks:
- Anomalies and Events: What tools can detect and alert IT security staff of anomalies (e.g., SIEM tools)?
- Continuous Monitoring: What tools or processes are needed to monitor the network for security events?
- Detection Process: What tools are required to detect security events, such as IDS?

 Response: The cybersecurity team should configure source IP address verification on the firewall and analyze spoofed IP addresses using tools like Wireshark or TCPdump for incoming ICMP packets. Implementing network monitoring software, such as SIEM tools (e.g., Splunk or LogRhythm), will help detect abnormal traffic patterns effectively.
 
4	Respond: Respond to threats and attacks:
- Planning: What action plans need to be in place for similar attacks?
- Communication: How will security response procedures be communicated to end users and IT staff?
- Analysis: What steps should be followed to analyze the response to a similar attack?
- Mitigation: What steps could mitigate the attack's impact (e.g., isolating resources)?
- Improvements: What can be improved to enhance future responses?

 Response: The cybersecurity team should develop a risk management plan for handling future incidents. This report will serve as a guide for responding to threats. In the event of an attack, the team will immediately inform end users about next steps and isolate affected systems to contain the spread of malicious activity. Critical systems and services will be prioritized for restoration, while network logs will be analyzed to identify suspicious behavior. A detailed report will be shared with upper management and, if required, legal authorities in compliance with regulations.

5	Recover: Restore affected systems or data:
- Recovery Planning: How will resources be restored?
- Improvements: Can the recovery process or systems be improved?
- Communication: How will restoration procedures be communicated to affected parties?

 Response: To address the ICMP flooding issue, a firewall should be used to block these attacks. The priority will be to restore critical network services, while non-critical networks may temporarily go offline. Once the ICMP flood subsides, non-critical systems and services can gradually be brought back online.
