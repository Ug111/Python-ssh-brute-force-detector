# Python SSH Brute Force Detection & Auth Log Analyzer
 ____ v1
|     |____ original_script.py
|____ v2/
|     |____ auth_log_analyzer_v2.py
|     |____ ssh_detection_report.txt
|     
|____ screenshots/
|     |____ hydra_attack.png
|     |____ detection_output.png
|
|____ README.md

## 📌 Overview of this Lab
This project was developed in a controlled virtual lab environment using Ubuntu and Kali Linux 
to simulate and detect SSH brute-force attacks through authentication log analysis

## 🎯 Goal
I built this to better understand howfailed log patterns can indicate malicious activities.

## SOC Use Case
This tool simulates a SOC detection workflow where authentication logs are analyzed to identify
brute-force attacks and potential account compromise.

## 🔍 what it does:
- Parses auth logs
- Tracks failed login attempts per IP
- Identifies suspicious activity
- Flags successful login after multiple failures

## 🧠 what i learned 
- Regex parsing for log analysis
- How attackers behave during brute-force attempts
- Structuring detection logic in Python

## ⚠️ Limitations
- Detection is not yet time-based
- No real-time monitoring

##  🚀 Next Steps

## Project Evaluation
Version 1 (v1)
The initial version focused on detecting repeated failed SSH login attempts
from authentication logs.

Version 2 (v2)
* Severity scoring
* Timestamp tracking
* User-target detection
* TXT report exporting
* Improved attack analysis
* Detection of successful  VS
  unsuccessful compromise attempts

This version was tested using simulated brute-force attacks from kali Linux with 
Hydra against an Ubuntu SSH server.

- implement time-based detection (e.g., x attempts in Y seconds)
- Improve reporting format
