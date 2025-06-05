Task 1 Result: Local Network Port Scan

-Identified my IP address as 10.0.2.15/24, so I used the IP range    10.0.2.0/24 for scanning.

-Installed and used Nmap to perform a TCP SYN scan with the command:
nmap -sS 10.0.2.0/24

Scan results:

-10.0.2.1 → Ports 80 (HTTP) and 443 (HTTPS) open

-10.0.2.3 → Port 22 (SSH) open

Observations:

-HTTP (port 80) is unencrypted and can expose data.

-SSH (port 22) can be a brute-force target if not secured.

-Saved the scan results as a text file using the -oN option.
