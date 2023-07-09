# This report is about how attacks at different OSI layers could compromise network security and affect the overall system.
## Application Layer
### What is the Application Layer 
The Application layer of the OSI model is responsible for providing services to end-user applications, such as email, web browsing, file transfer, and remote access. 
Application Layer attacks, including Cross-Site Scripting (XSS) or SQL injection, can compromise the security of web applications. XSS attacks can enable attackers to inject malicious scripts into web pages, potentially compromising user data or spreading malware. SQL injection attacks can manipulate database queries, leading to unauthorized data access or modification.

Attacks at the Application layer can compromise network security and affect the overall system in several ways - 

<details>
           <summary>Denial-of-Service (DoS) Attacks</summary>
           <p>Attackers can target specific applications by flooding them with an overwhelming amount of traffic, rendering them unavailable to legitimate users. This can disrupt business operations and impact the overall availability and performance of the network.</p>
</details>

<details>
           <summary>Cross-Site Scripting (XSS)</summary>
           <p>XSS attacks occur when an attacker injects malicious code into a trusted website or application, which then executes on the user's browser. This can lead to the theft of sensitive information, session hijacking, or even control over user accounts.</p>
         </details>
  
<details>
           <summary>SQL Injection</summary>
           <p>In an SQL injection attack, an attacker exploits vulnerabilities in an application's database query mechanism. By injecting malicious SQL statements, the attacker can manipulate the database, gain unauthorized access to sensitive data, modify or delete data, or execute arbitrary commands on the underlying system.</p>
         </details>

<details>
           <summary>Phishing and Social Engineering</summary>
           <p>Attackers often use deceptive techniques to trick users into divulging sensitive information like passwords or credit card details. These attacks usually occur via email, instant messaging, or fraudulent websites, and can compromise user accounts, leading to unauthorized access to the network.</p>
         </details>
  
<details>
           <summary>Man-in-the-Middle (MitM) Attacks</summary>
           <p>In a MitM attack, an attacker intercepts communication between two parties and can eavesdrop, modify, or inject malicious content into the communication stream. This can compromise the confidentiality, integrity, and authenticity of the transmitted data and can affect overall system security.</p>
         </details>
         
#### Mitigation Strategies
Mitigating attacks on the application layer of the OSI model necessitates the implementation of several security strategies to protect applications and the underlying infrastructure. An essential approach is to **adopt secure coding practices**, which involve techniques such as input validation, output encoding, and proper error handling. These practices can prevent common vulnerabilities such as code injection, cross-site scripting (XSS), or SQL injection. Additionally, **deploying Web Application Firewalls (WAF)** is crucial. WAF solutions can analyze incoming web traffic, identify potential threats, and block malicious requests or payloads targeting the application layer. **Employing intrusion detection and prevention systems** specific to web applications can also help detect and thwart attacks. Regular **security assessments and vulnerability scanning** are essential for identifying and patching application-level vulnerabilities. Keeping applications and associated *software up to date* with the latest security patches and updates is imperative. Lastly, **user education and awareness programs** can promote good security practices, such as using strong passwords, enabling multi-factor authentication, and exercising caution while interacting with web applications. By implementing these mitigation strategies, organizations can enhance the security posture of their applications and protect against attacks at the application layer.

> Attacks on the application layer can have severe consequences and compromise network security in various ways. For instance, SQL injection attacks can lead to unauthorized access to databases, enabling attackers to retrieve or manipulate sensitive information. Cross-Site Scripting (XSS) attacks can allow malicious scripts to be executed within users' browsers, leading to session hijacking, data theft, or website defacement. By exploiting vulnerabilities in web applications, attackers can gain remote code execution capabilities, granting them unauthorized access to the underlying systems and potentially compromising the entire network. Distributed Denial of Service (DDoS) attacks targeting the application layer can overwhelm servers, rendering applications and services inaccessible to legitimate users, causing significant disruption. Moreover, successful attacks such as session hijacking, man-in-the-middle attacks, or clickjacking can bypass authentication mechanisms, compromise user credentials, and enable further unauthorized access to network resources. These examples illustrate how attacks on the application layer can undermine network security, highlighting the importance of implementing robust security measures and conducting regular vulnerability assessments to protect against such threats.

## Presentation Layer
### What is Presentation Layer 
The presentation layer, also known as the “syntax layer”, is responsible for formatting and translating data into the format the application layer specifies. It is to say, it acts as the network’s data translator to ensure that the data sent out by the application layer is readable by the receiving system’s application layer. This OSI model layer communicates and interacts with: the application layer and the session layer. Presentation Layer attacks, like encryption attacks or manipulating data formats, can undermine the confidentiality and integrity of data. Successful encryption attacks can expose sensitive information, and manipulating data formats can lead to data corruption, unauthorized access, or execution of malicious code.


Attacks at the Presentation layer can compromise network security and affect the overall system in several ways - 

<details>
           <summary>Code Injection</summary>
           <p>Attackers attempt to inject malicious code into data streams or input fields that are processed by the presentation layer. This code can exploit vulnerabilities in the data formatting or rendering process, leading to unauthorized execution of arbitrary code.</p>
</details>

<details>
           <summary>Content Spoofing</summary>
           <p>In this type of attack, the attacker manipulates the presentation of data to deceive users. For example, an attacker may forge a website or application to make it appear legitimate and trick users into providing sensitive information.</p>
</details>

<details>
           <summary>Format String Attacks</summary>
           <p>These attacks target vulnerabilities in how applications handle format strings, which are placeholders used for formatting data. By manipulating the format string, an attacker can read or write arbitrary memory, leading to unauthorized data access or code execution.</p>
         </details>
  
<details>
           <summary>Brute Force Attacks</summary>
           <p>Attackers may attempt to guess or crack encryption keys or passwords used for data encryption or decryption in the presentation layer. By systematically trying various combinations, they aim to gain unauthorized access to sensitive data.</p>
         </details>

<details>
           <summary>Data Injection</summary>
           <p>Attackers can attempt to inject malicious or unexpected data into the presentation layer. This can lead to data corruption, unauthorized access, or exploitation of vulnerabilities in the processing or rendering of the injected data.</p>
         </details>

#### Mitigation Strategies

Mitigating attacks on the presentation layer of the OSI model requires the implementation of various security measures to protect the formatting, encoding, and presentation of data. One essential strategy is to **employ robust input validation and sanitization mechanisms** to ensure that data received at the presentation layer is properly validated and cleansed. This helps prevent code injection and other types of malicious input that can exploit vulnerabilities in data processing or rendering processes. Additionally, **applying proper output encoding techniques** is crucial to mitigate the risk of cross-site scripting (XSS) attacks. By encoding special characters and user-generated content, the risk of injecting malicious scripts into the presentation layer can be significantly reduced. **Implementing encryption and secure communication protocols**, such as TLS (Transport Layer Security), helps protect the confidentiality and integrity of data transmitted at the presentation layer.

> Attacks on the presentation layer can pose significant risks to network security, potentially compromising the confidentiality, integrity, and availability of data and services. For instance, code injection attacks targeting the presentation layer can exploit vulnerabilities in data formatting and rendering processes, leading to the execution of malicious code within applications. This can result in unauthorized access, data manipulation, or the compromise of sensitive information. Cross-Site Scripting (XSS) attacks at the presentation layer can allow attackers to inject and execute malicious scripts in users' browsers, enabling them to steal user credentials, initiate session hijacking, or perform other unauthorized actions. Additionally, denial-of-service (DoS) attacks on the presentation layer can overload and disrupt the processing and rendering of data, leading to application downtime and service unavailability. By compromising the presentation layer, attackers can undermine the overall security of the network and its applications, emphasizing the need for robust security measures such as input validation, secure coding practices, and regular security assessments to detect and mitigate vulnerabilities in this layer

## Session Layer
### What is Session Layer 
The session layer is the fifth layer of the OSI (Open Systems Interconnection) model. Its primary function is to establish, manage, and terminate communication sessions between two network devices. The session layer ensures reliable and orderly data exchange by providing mechanisms for session establishment, maintenance, synchronization, and recovery in case of failures.


Attacks at the Session layer can compromise network security and affect the overall system in several ways - 

<details>
           <summary>Session Hijacking</summary>
           <p>This attack involves an unauthorized individual gaining control over a legitimate user's session by intercepting or stealing session identifiers or tokens. The attacker can then impersonate the user and perform actions on their behalf.</p>
</details>

<details>
           <summary>Session Replay</summary>
           <p>In a session replay attack, the attacker captures and replays a previously recorded session to repeat the actions taken by the original user. This can enable the attacker to carry out unauthorized activities or access sensitive information.</p>
</details>

<details>
           <summary>Session Sidejacking</summary>
           <p>Also known as session eavesdropping, this attack occurs when an attacker intercepts and steals session cookies or tokens transmitted over an insecure network. The attacker can use the stolen credentials to hijack the session and gain unauthorized access.</p>
         </details>
  
<details>
           <summary>Resource Exhaustion</summary>
           <p>Attackers may attempt to exhaust session-related resources, such as session identifiers or connection state tables, leading to service degradation or denial of service.</p>
         </details>

<details>
           <summary>Session Prediction</summary>
           <p>Attackers may attempt to predict or guess valid session identifiers, typically through the analysis of patterns or weak randomization algorithms used in session identifier generation. Successful prediction can enable attackers to hijack sessions and gain unauthorized access.</p>
         </details>

#### Mitigation Strategies

Mitigating attacks on the session layer of the OSI model involves implementing various security measures to protect session establishment, maintenance, and termination processes. One key mitigation strategy is to implement **strong authentication mechanisms**, such as multi-factor authentication, to ensure secure session establishment. By verifying the identity of users or devices, the risk of unauthorized session initiation is minimized. **Employing encryption protocols**, such as SSL/TLS, helps protect session data during transmission, ensuring confidentiality and integrity. Regularly monitoring session activity and implementing session timeouts can help mitigate the risk of session hijacking or unauthorized access. **Implementing robust session management controls**, including secure session identifiers and strong session key generation algorithms, adds an additional layer of protection. It is also important to conduct regular security assessments to identify vulnerabilities and promptly apply patches or updates to session management software.

> While attacks directly targeting the session layer are less common, compromising the session layer can have significant implications for network security. Attacks such as session hijacking or man-in-the-middle attacks can result in unauthorized access to sensitive information or allow attackers to masquerade as legitimate users, compromising the integrity and confidentiality of network communications. By gaining control over sessions, attackers can bypass authentication mechanisms, perform unauthorized actions, or manipulate session parameters. Session layer attacks can also disrupt the establishment, maintenance, or termination of sessions, leading to service disruptions or denial of service. Additionally, exploiting vulnerabilities in session management can undermine the trust and reliability of the network, eroding user confidence and potentially leading to further security breaches in higher layers of the network stack.

## Transport Layer
### What is Transport Layer 
The Transport Layer is the fourth layer in the OSI (Open Systems Interconnection) model, responsible for reliable end-to-end communication between devices across a network. This layer ensures the delivery of data packets and provides error recovery, flow control, and congestion control mechanisms. The Transport Layer establishes and manages connections between devices, ensuring reliable data delivery. It segments and reassembles data into manageable units for transmission and handles end-to-end flow control. The primary protocols at this layer include TCP (Transmission Control Protocol) and UDP (User Datagram Protocol).

Attacks at the Transport layer can compromise network security and affect the overall system in several ways - 

<details>
           <summary>TCP SYN Flooding</summary>
           <p>This type of attack exploits the TCP three-way handshake process by sending a flood of SYN (synchronization) packets to overwhelm the target system's resources. The goal is to exhaust the system's ability to establish new connections, resulting in a denial-of-service (DoS) condition.</p>
</details>

<details>
           <summary>TCP Session Hijacking</summary>
           <p>In a session hijacking attack, an attacker intercepts and takes control of an existing TCP session between two hosts. By eavesdropping on the session or successfully predicting the sequence numbers, the attacker can impersonate one of the communicating parties, gain unauthorized access, or manipulate the transmitted data.</p>
</details>

<details>
           <summary>TCP Reset Attack</summary>
           <p>Also known as a TCP RST attack, this involves sending spoofed TCP reset packets to abruptly terminate an established TCP connection. This can disrupt communication between hosts, leading to service disruptions or session terminations.</p>
         </details>
  
<details>
           <summary>UDP Flood</summary>
           <p>In a UDP flood attack, the attacker floods the target system with a large volume of UDP packets. Since UDP is connectionless and does not have the same level of error checking as TCP, the goal is to overwhelm the target system's network resources and cause a DoS condition.</p>
         </details>

<details>
           <summary>Transport Layer Security (TLS)/Secure Sockets Layer (SSL) Attacks</summary>
           <p>These attacks exploit vulnerabilities in the TLS/SSL protocols used for secure communication. Examples include protocol downgrade attacks, where attackers force the use of weaker encryption protocols or cryptographic vulnerabilities, or exploiting implementation flaws in SSL/TLS libraries.</p>
         </details>This layer establishes a point-to-point connection between the source and the destination, ensuring that the data is transmitted in the correct order. It also performs flow control, error control, data reassembly, and segmentation. Transmission Control Protocol (TCP) and User Datagram Protocol (UDP) are examples of transport layer protocols.
Attacks in this layer are often conducted through vulnerable open ports identified by port scanning.
SYN flood attack :
                                      This is a type of DDoS attack that exploits the TCP three-way handshake. The attacker sends multiple synchronization (SYN) packets to every port of a server. The server acknowledges by sending a Synchronize-Acknowledge (SYN-ACK) message for each SYN packet. If the malicious client doesn’t send the final ACK packet as expected, it creates “half-open” sessions on the server. As the server’s ability to process requests becomes depleted, new requests and services to legitimate clients will be denied. If the SYN flood continues, the server will malfunction or crash. SYN flood attacks can be mitigated by allocating micro-blocks, as few as 16 bytes for a SYN request, and maintaining SYN cookies and RST cookies.


                              


Working Of SYN flood attack:
                                                      
SYN flood attacks work by exploiting the handshake process of a TCP connection. Under normal conditions, TCP connection exhibits three distinct processes in order to make a connection.
First, the client sends a SYN packet to the server in order to initiate the connection.
The server then responds to that initial packet with a SYN/ACK packet, in order to acknowledge the communication.
Finally, the client returns an ACK packet to acknowledge the receipt of the packet from the server. After completing this sequence of packet sending and receiving, the TCP connection is open and able to send and receive data.

To create denial-of-service, an attacker exploits the fact that after an initial SYN packet has been received, the server will respond back with one or more SYN/ACK packets and wait for the final step in the handshake. 

Here’s how it works:
The attacker sends a high volume of SYN packets to the targeted server, often with spoofed IP addresses.
The server then responds to each one of the connection requests and leaves an open port ready to receive the response.
While the server waits for the final ACK packet, which never arrives, the attacker continues to send more SYN packets. The arrival of each new SYN packet causes the server to temporarily maintain a new open port connection for a certain length of time, and once all the available ports have been utilized the server is unable to function normally.



Smurf attack :
                                  Named after a popular toy figure from the 1980s that appeared to be everywhere, the Smurf attack is also a type of a DDoS attack. This attack is carried out by generating fake ICMP Echo request (PING) packets to an IP broadcast network using the targeted server`s IP address as the source IP address. With so many ICMP responses, seeming to come from everywhere, the target server becomes overwhelmed and is bought down. Inspection of incoming, traffic and blocking illegal ICMP responses will limit the chances of a Smurf attack.

Internet Control Message Protocol (ICMP) is a form of DDoS attack that overloads network resources by broadcasting ICMP echo requests to devices across the network. Devices that receive the request respond with echo replies, which creates a botnet situation that generates a high ICMP traffic rate. 
                                  As a result, the server is flooded with data requests and ICMP packets, which overwhelm the computer network and make it inoperable. This can be particularly problematic for distributed computing systems, which allow devices to act as computing environments and enable users to access resources remotely.

A smurf attack works through the following three-step process:
The DDoS Smurf malware creates a network data packet that attaches to a false IP address. This is known as spoofing.
The packet contains an ICMP ping message, which commands network nodes to send a reply.

This process, known as ICMP echoes, creates an infinite loop that overwhelms a network with constant requests.

Prevent Smurf Attack:
                                         A Smurf Attack implies 3 players: the hacker, the intermediary / the amplifier, the victim. In order for the attack to start, the intermediary has to let a source-spoofed IP packet leave its network. Therefore, prevention has to be done on two levels: you must avoid being attacked and you must avoid being used to launch an attack. 
To avoid being the amplifier, you should disable IP-directed broadcast on the router – this will make it deny the broadcast traffic to the internal network from other networks. You can also try to apply an outbound filter to your perimeter router, as well as configuring hosts and routers not to respond to ICMP echo requests. 
To avoid being the victim, you should:

                                                               have a prevention strategy based on traffic network monitoring that can detect any oddments – like packet volume, behaviour and signature. This could help you stop a Smurf Attack before it even begins. 
– install an antivirus and an anti-malware solution and protect your servers with network firewalls or specialized web application firewalls. You could try for that matter Gen Endpoint Antivirus. Its firewall can help you prevent incoming attacks, while the AV uses 4 stages of scanning (Local File/Signature & Registry Scanning; Real-time Cloud Scanning; Sandbox and Backdoor Inspection; Process Behaviour-based Scanning) to detect and identify even the most advanced threats. Our solution’s firewall also offers full management of the windows firewall and device Isolation in case of major outbreaks, enabling IT to lockdown departments quickly, according to the NIST AC-7 Policy regarding Authentication Failures. 

#### Mitigation Strategies

Mitigating attacks on the transport layer of the OSI model requires implementing various security measures to protect the reliable transmission of data between network hosts. One key strategy is to *implement secure transport protocols* such as Transport Layer Security (TLS) or Secure Socket Layer (SSL). These protocols encrypt data during transmission, ensuring confidentiality and integrity, and protect against attacks that aim to intercept or tamper with data in transit. It is crucial to keep the transport layer protocols and their implementations up to date with the latest security patches to address known vulnerabilities. *Implementing proper network segmentation and access controls* helps prevent unauthorized access to network resources and protects against attacks that target the transport layer. Intrusion detection and prevention systems (IDPS) can monitor network traffic, detect suspicious activities, and block potential attacks at the transport layer. Additionally, *implementing strong authentication mechanisms and access controls* helps ensure that only authorized hosts can establish connections and access network resources.

> Attacks on the transport layer can have severe implications for network security, compromising the confidentiality, integrity, and availability of data and services. For example, TCP SYN flooding attacks can overwhelm a system's resources, leading to denial-of-service (DoS) conditions and rendering services inaccessible to legitimate users. Session hijacking attacks targeting the transport layer can enable unauthorized access, data tampering, or the impersonation of legitimate communication parties, potentially leading to unauthorized disclosure of sensitive information or unauthorized actions. Manipulating or disrupting transport layer protocols, such as TCP or UDP, can result in the disruption of network communication, loss of data, or the injection of malicious payloads into network streams.
        
