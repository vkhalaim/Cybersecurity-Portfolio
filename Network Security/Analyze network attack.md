# Cybersecurity Incident Report: Analyze Network Attacks
> Network attacks.

> Please visit this [link](https://www.coursera.org/learn/networks-and-network-security?specialization=google-cybersecurity) for further information. 

## Scenario

You work as a security analyst for a travel agency that advertises sales and promotions on the company’s website. The employees of the company regularly access the company’s sales webpage to search for vacation packages their customers might like. 

One afternoon, you receive an automated alert from your monitoring system indicating a problem with the web server. You attempt to visit the company’s website, but you receive a connection timeout error message in your browser.

You use a packet sniffer to capture data packets in transit to and from the web server. You notice a large number of TCP SYN requests coming from an unfamiliar IP address. The web server appears to be overwhelmed by the volume of incoming traffic and is losing its ability to respond to the abnormally large number of SYN requests. You suspect the server is under attack by a malicious actor. 

You take the server offline temporarily so that the machine can recover and return to a normal operating status. You also configure the company’s firewall to block the IP address that was sending the abnormal number of SYN requests. You know that your IP blocking solution won’t last long, as an attacker can spoof other IP addresses to get around this block. You need to alert your manager about this problem quickly and discuss the next steps to stop this attacker and prevent this problem from happening again. You will need to be prepared to tell your boss about the type of attack you discovered and how it was affecting the web server and employees.

| Section 1: Identify the type of attack that may have caused this  network interruption |  |
| :---- | ----- |
| One potential explanation for the website's connection timeout error message is:  The logs show that: abnormal number of SYN requests from 203.0.113.0
| This event could be: DoS attack with SYN flood was performed  |  |
|  |  |

| Section 2: Explain how the attack is causing the website to malfunction |
| :---- |
| When website visitors try to establish a connection with the web server, a three-way handshake occurs using the TCP protocol. Explain the three steps of the handshake: 
  1\. Client send SYN packet to the server
  2\. Server sends back SYN-ACK packet to the client
  3\.The last step when a client sends back an ACK packet. Now TCP connection is established
|  Explain what happens when a malicious actor sends a large number of SYN packets all at once: When a malicious actor sends a large amount of SYN packets this can establish a lot of responses with SYN-ACK and the server will wait for an answer from the malicious actor. Since the amount of resources is limited this can lead to denial of service.
|  Explain what the logs indicate and how that affects the server: The logs indicates that after certain amount of requests, the server is not available to continue respond to the requests, so DoS attack was successful.  |
