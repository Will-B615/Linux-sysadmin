# Linux Junior System Engineer Lab Portfolio Entry 

  

## Summary 

  

This portfolio entry documents a first-day sysadmin lab on an Ubuntu server, highlighting hands-on engagement with real-world Linux administration tasks within a small enterprise environment. The scenario demonstrates secure server access, user and group management, directory permissioning, process automation via scripting, safe script execution and error handling, and comprehensive system resource auditing. Each step includes terminal output and evidence, adhering to SOC-style reporting and best practices for repeatability and security compliance. 

  

## Highlighted Linux Skills 

  

- **Secure Server Access:** Used SSH for authenticated login and remote management. 

- **User & Group Management:** Created and managed user accounts and groups to support department separation and access control. 

- **Directory & Permission Management:** Set up directories with proper ownership and group privileges, using `chmod` and `chown` for strong access enforcement. 

- **Scripting & Automation:** Developed bash scripts to automate software installation (`figlet`, `lolcat`) and implemented executable permissions for deployment repeatability. 

- **Safe Script Download & Execution:** Downloaded external scripts securely with `wget`, managed execution permissions, and redirected error logs for auditing. 

- **System Auditing:** Gathered and recorded disk, memory, and CPU information using `fdisk`, `df -h`, `cat /proc/meminfo`, and `cat /proc/cpuinfo` for hardware inventory and resource monitoring[file:2]. 

  

## SOC-Style Incident Entry 

  

| Timestamp | Task | Command/Evidence | Outcome | 

|-----------|------|------------------|---------| 

| Day 1 | SSH Login | `ssh student@server` | Authenticated access | 

<img width="929" height="297" alt="Screenshot 2025-10-19 081429" src="https://github.com/user-attachments/assets/c08c2ff0-74cb-4cc4-bbce-1ce3cd831ae2" />

---
| Day 1 | User/Group Setup | `groupadd humanresources; useradd robbie -g humanresources -m -s /bin/bash` | User created and added to group| 

<img width="1012" height="150" alt="Screenshot 2025-10-19 082021" src="https://github.com/user-attachments/assets/9854be3b-7f6e-492f-b2c4-123ee50d54bf" />

---
| Day 1 | Directory Management | `mkdir /var/ieke4; chown mitchellcustomerservice /var/ieke4; chmod 770 /var/ieke4` | Directory created with proper permissions | 

<img width="796" height="207" alt="Screenshot 2025-10-19 082803" src="https://github.com/user-attachments/assets/da7eef65-3a91-4b60-ab05-42f039197d5e" />

---
| Day 1 | Automation Scripting | `nano clearwater.sh; chmod +x clearwater.sh; ./clearwater.sh` | Tools installed via script | 

<img width="1003" height="301" alt="Screenshot 2025-10-19 084220" src="https://github.com/user-attachments/assets/0b2f0bc7-3634-4c7c-a5a1-d5eb9d8f88cb" />

<img width="1012" height="338" alt="Screenshot 2025-10-19 084543" src="https://github.com/user-attachments/assets/ef849f0c-2948-4ee9-8718-eca19c21baaf" />

---

| Day 1 | Safe Script Execution | `wget https://devops.lab/austin.sh; chmod +x austin.sh; ./austin.sh 2> austin-errors.txt` | Script run with errors logged | 

<img width="998" height="339" alt="Screenshot 2025-10-19 085020" src="https://github.com/user-attachments/assets/e4792a24-efc8-49f8-8557-1e2cbe028159" />

<img width="1002" height="669" alt="Screenshot 2025-10-19 085333" src="https://github.com/user-attachments/assets/a8abf079-3030-432b-bd16-cb5e74f0b408" />

---

| Day 1 | System Audit | `fdisk -l; df -h; cat /proc/meminfo; cat /proc/cpuinfo` | Disk 11 GiB, RAM 2GB, CPU info gathered | 

<img width="998" height="123" alt="Screenshot 2025-10-19 090705" src="https://github.com/user-attachments/assets/bf56a211-4744-4755-a13c-ea35b74aea9f" />

<img width="992" height="310" alt="Screenshot 2025-10-19 090746" src="https://github.com/user-attachments/assets/e88b3347-cf2e-4f5c-9f7e-27c732a6c385" />

<img width="785" height="240" alt="Screenshot 2025-10-19 090948" src="https://github.com/user-attachments/assets/7cf76882-7ab2-46b6-baaf-cbc35e171b6a" />

<img width="787" height="298" alt="Screenshot 2025-10-19 091423" src="https://github.com/user-attachments/assets/af40a825-ec1b-4cef-82c4-ea1e58ac1f9d" />

<img width="958" height="318" alt="Screenshot 2025-10-19 091608" src="https://github.com/user-attachments/assets/2ca61813-a1a9-4c31-82fe-0245a79e17f8" />

---




  

## Key Outcomes 

  

- Demonstrated readiness to support onboarding tasks and secure setup for new Linux environments. 

- Applied repeatable and secure methods for typical SOC and sysadmin procedures. 

- Ensured compliance with best practices in access control, process automation, and hardware resource management[file:2]. 

  

--- 

 
