FTP vs. SFTP Packet Analysis 

Project link: https://docs.google.com/document/d/1IgEk4XneObG4G5ky6nPWK9pELmML_jgreA7kEpRkQjc/edit?usp=drive_link

Focus: Traffic Analysis, Protocol Security, and Packet Sniffing.

Overview: Conducted a comparative analysis of file transfer protocols to demonstrate the risks of cleartext communication. Used Wireshark to capture and analyze live network traffic on a Kali Linux machine.

The Experiment:

The Insecure Test (FTP): Configured vsftpd and logged in as a user. Captured the traffic and extracted the password (Request: PASS) in plain text from the TCP stream, proving the protocol is unsafe.

The Secure Test (SFTP): Repeated the login using SSH (Port 22). The Wireshark capture showed only encrypted ciphertext, confirming that credentials and data were protected from interception.

Tools Used: Kali Linux, Wireshark, vsftpd, OpenSSH.