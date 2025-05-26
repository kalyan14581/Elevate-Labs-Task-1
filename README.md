# Elevate-Labs-Task-1

Task 1: Scan Your Local Network for Open Ports:

    -- Install Nmap and wireshark from offical website 
    --Take your local wifi ip address and open up to Nmap do a normal scan so that you will get an ideal hoe to scan an ip address
    --Now use a cmd call nmap -sS which is used to perform TCP SYN scan 
    --After  the compeltion of your scan note down the ip's connected to same network
    -- Now go to Wireshare and capture the network traffic in wifi and compare the ip's you have found in nmap scan and see what ports are open   
    
![Screenshot 2025-05-26 175238](https://github.com/user-attachments/assets/1ce5a2b2-1c31-4c2b-a1f8-580d389565c7)
![Screenshot 2025-05-26 172537](https://github.com/user-attachments/assets/396257b8-b7d8-4fa8-aa94-28ced9ae7610)
![Screenshot 2025-05-26 182514](https://github.com/user-attachments/assets/f16c5916-5fe8-471c-8811-a2f21a239664)

Common Services running:

          --21/tcp (FTP): File Transfer Protocol; used for file transfers (risk: weak authentication).
          --22/tcp (SSH): Secure Shell; remote access (risk: brute-force attacks if not secured).
          --23/tcp (Telnet): Remote access (unencrypted, high risk: avoid using).
          --25/tcp (SMTP): Simple Mail Transfer Protocol; email sending (risk: spam or phishing if misconfigured).
          --53/tcp-udp (DNS): Domain Name System; name resolution (risk: DNS spoofing).
          potential security risks from open ports--80/tcp (HTTP): Web traffic (risk: web vulnerabilities like XSS, SQL injection).
          --443/tcp (HTTPS): Secure web traffic (risk: SSL/TLS misconfigurations).
          
This are the ports that i have got from scanning my local ip
And I have also mentioned  potential security risks for this open ports:

          --135 (msrpc): Used for Microsoft RPC, enabling inter-process communication in Windows; often targeted by malware.
          --139 (netbios-ssn): NetBIOS over TCP for legacy Windows file/printer sharing; vulnerable to enumeration and SMB exploits.
          --443 (https): Secure HTTP for web traffic; risks include SSL/TLS vulnerabilities if not properly configured.
          --445 (microsoft-ds): SMB for modern Windows file sharing; a frequent target for ransomware (e.g., EternalBlue).
