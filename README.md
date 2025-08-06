# Phishing Email Analysis Report# Elevate-Labs

# 🔍 Task Objectives

Obtain a real phishing‑style email sample and analyze its sender details, headers, links, language, and formatting to identify and summarize key phishing indicators.

# 🧪 Tools Used

Kali Linux

Online Email Header Analyzer (mxtoolbox)



# Source of Sample Phishing Email
The sample phishing email used in this task was downloaded from the following open-source repository:

🔗[https://github.com/rf-peixoto/phishing_pot] (Github Sample Repository)

- Basic Information

| Field  | Value |
| ------------- | ------------- |
| File Name  | sample-100.eml  |
| Data Analyzed | 2025-08-06  |


# Steps Taken

1. Downloaded `sample-100.eml` from an open-source repository.  
2. Opened the sample email in Thunderbird on Kali Linux.  
3. Copied the full email header from Thunderbird.  
4. Submitted the header to MXToolbox’s header analyzer.  
5. Examined the following header fields and indicators:
   - **From**, **Reply-To**, **Return-Path**  
   - SPF record status  
   - Subject line and language used  
   - Date/time information  
6. Identified and summarized all indicators of phishing.  
7. Captured screenshots of the header analysis report for documentation.

# 🔎Header Analysis

| Field  | Details |
| ------------- | ------------- |
| From  | zonnepaneel@appjj.serenitepure.fr  |
| Reply-To | news@aichakandisha.com  |
| Return Path | return@dturm.de  |
| Sender | zonnepaneel@appjj.serenitepure.f  |
| SPF None | None (protection.outlook.com: dturm.de does not designate permitted sender hosts) |
| Subject | 🔋 Zonnepanelen voor een goede prijs  |
| Date | Thu, 3 Nov 2022 04:56:15 +0000|

# 📸 Screenshots

Generated report by MXheaderanaalyser: 


![ss1](https://github.com/user-attachments/assets/1c305ef6-6f52-40b1-b24d-615f0ec80876)



![ss2](https://github.com/user-attachments/assets/754659d1-3e92-4e03-aec7-27af3825b3a4)



# Recommendation:
Do not interact with the similar mail. Mark it as phishing and report it to your IT/security team.

# ⚠️ Note:

This project is intended for educational and ethical use only. 

This analysis is for educational purposes only. No malicious activity is performed or encouraged.
