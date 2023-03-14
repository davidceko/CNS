# Lab Title: Man-in-the-middle attacks (ARP spoofing)

## Challenge Answers

- **Challenge 1:** [Insert answer here, i.e., a Chuck Norris fact]
- **Challenge 2:** [Insert answer here, i.e., a `password` to unlock the next lab]

## Other Relevant Information

[Insert here, if applicable]

## Lab Prep Questions and Answers

1. What is the *Address Resolution Protocol (ARP)*, and what is its role in a network?
    - Address Resolution Protocol (ARP) is a protocol that connects IP address to a fixed physical machine address - media access control (MAC) address, in a local-area network.
2. What is a *Man-in-the-Middle (MitM)* attack, and how does ARP spoofing enable it?
    - Man-in-the-middle (MITM) attack describes a situations in which an attacker intercepts communication between computers by convincing them that they are communicating directly. The attacker is able to take over the entire communication without the knowledge of its participants. ARP Spoofing enables the attacker to link his MAC address with the IP address of a legitimate computer on the network that he wants to impersonate. The attacker interrupts direct communication between computers and intercepts the traffic between them.
3. How does an attacker use ARP spoofing to intercept network traffic?
    - The attacker links his MAC address with the IP address of a legitimate computer on the network that he wants to impersonate.
4. How is the *cookie* used to derive the encryption/decryption key?
    - The cookie is used to derive encryption/decryption key. Key derivation function (KDF) scrypt is used.
5. What REST API request do you need to send to the *crypto oracle* the secret cookie?
    - GET /arp/cookie
6. How do you obtain the authentication token?
    - The authentication token is obtained from the c*rypto oracle* server. It is necessary to authenticate with our username and password.
7. How do you use the authentication token to obtain the cookie?
    - To successfully send a REST API request to the *crypto oracle server,* an authentication token is necessary. Only then can we obtain the cookie.
8. What encryption mode is used to encrypt the challenge in this lab?
    - AES-CBC (CBC encryption mode with AES cipher)
9. What tool can you use to capture network traffic on a local network interface?
    - tcpdump