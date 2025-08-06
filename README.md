# Phishing Email Analysis Report# Elevate-Labs

# 🔍 Task Objectives

Obtain and analyze a sample phishing email

Identify spoofed sender details

Inspect email headers using tools

Detect suspicious links or file attachments

Recognize urgent or threatening language

Check for URL mismatches

Spot spelling/grammar issues

Summarize all phishing indicators


# 🧪 Tools Used

Kali Linux

Online Email Header Analyzer (mxtoolbox)



# 📥 Source of Sample Phishing Email
The sample phishing email used in this task was downloaded from the following open-source repository:

🔗[https://github.com/rf-peixoto/phishing_pot] (Github Sample Repository)


# Summary of Steps Taken

Downloaded a sample phishing email (.eml file) from an Opensource GitHub repository.

Opened the email using Thunderbird on Kali Linux.

Copied the email header from Thunderbird.

Analyzed the header using MXToolbox Header Analyzer.

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


# Phishing Traits Identified

Spoofed sender email address (support@micros0ft.com)

External fake domain used in URL

Urgent action language to create panic

Spelling inconsistency (e.g., "Micros0ft")

Grammar mistakes and unnatural phrasing
