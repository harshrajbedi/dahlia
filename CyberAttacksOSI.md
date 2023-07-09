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
