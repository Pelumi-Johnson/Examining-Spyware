# 🧪 Examining Spyware (ANY.RUN Sandbox Analysis)

![Badge](https://img.shields.io/badge/Network%20Security-Malware%20Analysis%20%7C%20Sandbox-blue?style=for-the-badge)

📄 **Full Lab Report:**  
👉 [Click here to open the complete lab report](https://github.com/Pelumi-Johnson/Examining-Spyware/blob/main/Examining%20Spyware.pdf)

## 📌 Project Overview
This UMGC lab focuses on safely examining a suspected spyware executable in a controlled sandbox environment. The goal is to run the file in isolation, observe process behavior, review network/HTTP activity, and determine whether the file shows malicious indicators. 

---

## 🧠 Course Info
- **Institution:** University of Maryland Global Campus (UMGC)  
- **Course:** CMIT 320 Network Security
- **Lab Title:** Examining Spyware
- **Date:** January 13, 2026

---

## 🎯 Objective
Safely examine and analyze potential spyware behavior using a sandbox. Execute a file in isolation, monitor system and network activity, and determine whether the file exhibits malicious characteristics. 

---

## 🧰 Tools & Environment
- **uCertify Virtual Lab (Windows 10)**  
- **Google Chrome**
- **ANY.RUN Interactive Malware Analysis Sandbox**
- **Executable:** `write.exe`  
- **Monitoring Focus:**
  - Process tree 
  - Child processes  
  - HTTP requests   
  - Network activity 

---

## ✅ Lab Walkthrough (What I Did)

### Step 1: Launch and Configure the Sandbox
- Opened **Google Chrome** in the Windows 10 uCertify VM  
- Navigated to `https://app.any.run`  
- Signed into ANY.RUN using provided credentials  
- Selected **Submit File / Email** to begin a new analysis 

### Step 2: Upload the Executable
- In the Open dialog box, navigated to **Local Disk (C:)**  
- Searched for **`write.exe`** and selected it  
- Confirmed the file was uploaded for analysis
  
### Step 3: Run the Analysis
- Verified the environment (Windows 10 64-bit)  
- Started execution by selecting **Run a public analysis**

### Step 4: Monitor Processes
Observed the **Processes** pane during execution:
- `write.exe` ran as the **primary process**
- `wordpad.exe` appeared as a **child process**
- No additional or suspicious processes were observed
  
### Step 5: Review Network & HTTP Activity
Checked the **HTTP Requests** tab:
- Multiple **GET** requests were observed
- All returned **200 OK**
- No suspicious domains, abnormal traffic, or malicious indicators were detected 

### Step 6: Confirm Results
ANY.RUN summary reported:
- **Status:** No threats detected
- **Execution behavior:** Normal
- **Network activity:** Benign
- File did not demonstrate spyware or malicious behavior  

---

## 📊 Results Summary
| Category | Observation |
|---------|-------------|
| Primary process | `write.exe`
| Child process | `wordpad.exe`
| HTTP activity | GET requests, **200 OK** 
| Threat verdict | **No threats detected** 

---

## 🧾 Conclusion
This lab reinforced the importance of sandbox environments for spyware/malware analysis. By executing `write.exe` in an isolated environment, I was able to safely monitor process behavior and network activity without risking a production system. The analysis confirmed the file did not exhibit spyware characteristics.

---

## 🔑 Key Takeaways
- Sandbox environments are essential for safely analyzing unknown files.   
- Process trees help identify legitimate vs suspicious execution behavior. 
- Network + HTTP monitoring is critical for detecting spyware activity.
- A **“no threats detected”** result is still a valid analytical outcome. 

---

## 📎 Evidence
👉 [**Full UMGC Lab Report PDF**](https://github.com/Pelumi-Johnson/Examining-Spyware/blob/main/Examining%20Spyware.pdf)

