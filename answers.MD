## Snapped Phishing-Line Step by Step Documentation and Answers

### 1) Examine the firewall logs. What external IP performed the most reconnaissance?

> Since we are looking for port scans, I looked for blocked connection attempts in the logs, then filtered for the source IP and
sorted by count.

![Question 1 Screenshot](screenshots/q1.png)

### 2) In the firewall log, Which internal host was targeted by scans?
> For this I summarized which destination IP received the most hits. 

![Question 1 Screenshot](screenshots/q2.png)

### 3) Which username was targeted in VPN logs?
> In the VPN logs, I filtered for the attacker IP and manually searched in logs.

![Question 1 Screenshot](screenshots/q3.png)

### 4) What internal IP was assigned after successful VPN login?
> I manually searched the VPN logs using the previous command to see what IP address they first received.

![Question 1 Screenshot](screenshots/q4.png)

### 5) Which port was used for lateral SMB attempts?
> The port used for SMB is 445.

### 6) In the IDS logs, which host beaconed to the C2?
> Looking at the IDS logs, filtered for C2 and observed the source IP.

![Question 1 Screenshot](screenshots/q6.png)

### 7) During the investigation, which IP was observed to be associated with C2?
> Looking at the IDS logs, filtered for C2 and observed the destination IP.

![Question 1 Screenshot](screenshots/q7.png)

### 8) Which host showed the exfiltration attempts?
> Looking at the IDS logs, filtered for "Exfiltration" and observed the source IP.

![Question 1 Screenshot](screenshots/q8.png)


