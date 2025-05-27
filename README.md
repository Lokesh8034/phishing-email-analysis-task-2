# Phishing Email Analysis - Cyber Security Internship Task 2

## Overview

This project focuses on analyzing a phishing email sample to identify common phishing characteristics and investigate suspicious details using IP lookup tools and email threat analysis techniques.

---

## Objective

* Analyze a phishing email sample (image format)
* Identify phishing traits such as suspicious sender, urgency, spoofing, and brand impersonation
* Perform IP lookups to validate sender information
* Document findings and conclusions

---

## Tools Used

* IP lookup services (IP2Location, ipinfo.io, DB-IP, IPregistry, IPGeolocation, ipapi.co)
* Email header analysis tools (e.g., [MxToolbox Email Header Analyzer](https://mxtoolbox.com/EmailHeaders.aspx))
* Basic knowledge of phishing characteristics and threat indicators

---

## What We Did

* Obtained a phishing email sample in image format
![image](https://github.com/user-attachments/assets/ec2ce9c8-ff64-47be-954e-38d3b607fcb6)
* Identified phishing traits such as:

  * Sender address not matching legitimate domain (`support@msupdate.net`)
  * Urgent language prompting immediate action (password reset)
  * Suspicious links leading to fake login pages
  * Poor grammar and spelling errors
* Conducted IP lookup on the IP address `77.196.86.10` found in the email links
* Analyzed IP data from multiple services revealing multiple inconsistent locations in France
* Acknowledged limitations due to missing email headers (image format only)
* Explained what email headers would reveal if available, including SPF/DKIM/DMARC status

---

## Email Analysis Summary

| Indicator            | Details                                                             |
| -------------------- | ------------------------------------------------------------------- |
| **Sender Email**     | [support@msupdate.net](mailto:support@msupdate.net) (not Microsoft) |
| **Urgency**          | High - prompts password reset                                       |
| **Suspicious Links** | Likely fake login pages                                             |
| **Grammar/Language** | Poor grammar and broken sentences                                   |

---

## IP Lookup Results

| Tool          | City                 | Region              | ISP             |
| ------------- | -------------------- | ------------------- | --------------- |
| IP2Location   | Boulogne-Billancourt | Ile-de-France       | SFR SA          |
| ipinfo.io     | Tours                | Centre              | Not available   |
| DB-IP         | Paris                | Ile-de-France       | SFR User Data   |
| IPregistry    | Boulogne-Billancourt | Ile-de-France       | DSL - End Users |
| IPGeolocation | Paris                | Ile-de-France       | LDCOM NET       |
| ipapi.co      | Tours                | Centre-Val de Loire | SFR SA          |

**Conclusion:** The IP address does not belong to Microsoft and originates from locations inconsistent with the recipient's typical activity, indicating a strong phishing signal.

---

## Missing Email Headers

Due to the email being in image format, the following analysis could not be performed but would normally include:

* Email `Received` path tracing
* `Return-Path` verification
* SPF, DKIM, and DMARC authentication results

---

## Final Notes

* This phishing email displays multiple clear signs of a fraudulent Microsoft alert
* IP data and sender information strongly suggest a phishing attempt
* The report serves as documentation for the internship’s Task 2 submission

---

## License

This project is for educational purposes under the Cyber Security Internship program.

---
