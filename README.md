# Cybersecurity-Portfolio
Path to Junior SOC Analyst: Documenting technical labs, incident analysis, and problem-solving strategies.
# 🛡️ Cybersecurity Learning Journey — From Foundations to SOC

I am building my path toward becoming a **Junior SOC Analyst**, focusing on real-world skills in Linux, networking, and security analysis. This repository documents my hands-on progress, technical breakthroughs, and my evolving security mindset.

---

### 🎯 Current Focus
*   **Linux Fundamentals:** System navigation, file structures, and command-line efficiency.
*   **Access Control:** Understanding SSH authentication, permissions, and identity management.
*   **SOC Perspective:** Developing a log-analysis mindset and structured problem-solving.
*   **Networking:** Mastering the fundamentals of HTTP/HTTPS, headers, and data flow.

### 🛠️ Technical Toolbelt
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![Bash](https://img.shields.io/badge/Shell_Script-121011?style=for-the-badge&logo=gnu-bash&logoColor=white)
![SSH](https://img.shields.io/badge/SSH-000000?style=for-the-badge&logo=openssh&logoColor=white)
![Git](https://img.shields.io/badge/GIT-E44C30?style=for-the-badge&logo=git&logoColor=white)

---

### 💡 Breakthrough Highlights
| Challenge | The Obstacle | The "Aha!" Moment | Key Takeaway |
| :--- | :--- | :--- | :--- |
| **Bandit 13** | Localhost login blocked | Realized I had to transfer the private key via `SCP` to my local machine. | Private keys require strict `600` permissions to be valid. |
| **Natas 4** | Referer Spoofing | Shell threw errors due to special characters in the password. | Wrap credentials in single quotes `' '` to prevent shell expansion. |

---
### 📂 Detailed Command Logs
*   [View my step-by-step Bandit Lab Logs](./lab-logs/bandit-logs.md)

### 🚀 Featured Lab Analysis
#### **The SSH Identity Pivot (Bandit Level 13)**
*   **The Problem:** Trying to login to a restricted local service while physically on the server.
*   **The Analysis:** Identified that security policies blocked internal SSH loops. Analyzed file permissions and moved the target key to a local environment.
*   **The Result:** Successfully established a remote connection by satisfying SSH's strict security requirements.

---

### ⚡ Daily Discipline & Goals
*   **Consistency:** Minimum 1 hour of active lab work/study per day.
*   **Target:** Transitioning to **TryHackMe SOC Level 1** and **Blue Team Labs Online**.
*   **Goal:** Secure a Junior SOC Analyst internship by demonstrating documented technical proficiency.
