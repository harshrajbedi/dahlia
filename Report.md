Presentation layer | 6
The presentation layer, also known as the “syntax layer”, is responsible for formatting and translating data into the format the application layer specifies. It is to say, it acts as the network’s data translator to ensure that the data sent out by the application layer is readable by the receiving system’s application layer.
This OSI model layer communicates and interacts with: the application layer and the session layer.

The most common security attack on the presentation layer is: a phishing attack. 
Phishing attacks are the practice of sending fraudulent messages that appear to come from a trusted source. It is usually performed through email. The goal is to steal sensitive data like credit card and login information or install malware on the victim’s machine. Phishing is a common type of cyber-attack that everyone should learn about in order to protect themselves.

Attack vectors: SSL hijacking, encryption downgrade attacks, decryption attacks, encoding attacks, DDoS attacks

Mitigation: offload the SSL from the origin infrastructure and inspecting the application traffic for signs of attack traffic or violations of policy at an applications delivery platform (ADP). A good ADP will also ensure that your traffic is then re-encrypted and forwarded back to the origin infrastructure.

CASE STUDIES

1.  Facebook and Google
Between 2013 and 2015, Facebook and Google were tricked out of $100 million due to an extended phishing campaign. The phisher took advantage of the fact that both companies used Quanta, a Taiwan-based company, as a vendor. The attacker sent a series of fake invoices to the company that impersonated Quanta, which both Facebook and Google paid.

 Eventually, the scam was discovered, and Facebook and Google took action through the US legal system. The attacker was arrested and extradited from Lithuania, and, as a result of the legal proceedings, Facebook and Google were able to recover $49.7 million of the $100 million stolen from them.


2. Ubiquiti Networks
In 2015, Ubiquiti Networks, a computer networking company based in the US, was the victim of a BEC attack that cost the company $46.7 million (of which they expected to recover at least $15 million). The attacker impersonated the company’s CEO and lawyer and instructed the company’s Chief Accounting Officer to make a series of transfers to close a secret acquisition. Over the course of 17 days, the company made 14 wire transfers to accounts in Russia, Hungary, China, and Poland.

The incident only came to Ubiquiti’s attention when it was notified by the FBI that the company’s Hong Kong bank account may have been the victim of fraud. This enabled the company to stop any future transfers and attempt to recover as much of the $46.7 million stolen as possible (which represented roughly 10% of the company’s cash position).
