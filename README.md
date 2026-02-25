# Healthcare-Claims-Processing-Failure-Detection-Platform


Project Overview:
I built a monitoring and alerting system for healthcare claim processing in production. The goal was to track claim-related logs and detect failures in real time to avoid delays and revenue impact.

Problem Statement:
There was no automatic way to detect CLAIM errors. Issues were identified manually by checking logs, which delayed incident response.

Objective:
Centralize claim logs
Detect CLAIM failures automatically
Send real-time alert notifications
Reduce manual monitoring effort

Technologies Used:
Microsoft Azure
Azure Monitor
Log Analytics
KQL
Linux Syslog

Implementation:
I configured Syslog ingestion to Log Analytics and wrote KQL queries to filter CLAIM-related logs. I created a alert in Azure Monitor that triggers when a CLAIM error appears. I connected an email action group for notifications.

Testing & Validation:
I generated test logs from the VM using the logger command and verified that alerts were triggered successfully.

Results & Impact:
The system now detects claim failures automatically and sends alerts in real time. This improves incident response time and ensures smoother healthcare claim processing.

Conclusion:
This project helped me understand production monitoring, log analysis, and alert configuration in a real-world healthcare environment.
