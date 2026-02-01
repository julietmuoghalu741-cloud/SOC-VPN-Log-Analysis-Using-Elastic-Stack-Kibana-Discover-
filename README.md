SOC-VPN-Log-Analysis-Using-Elastic-Stack-Kibana-Discover-
This project demonstrates how a SOC analyst ingests and analyzes VPN log data using Splunk SIEM. The objective was to simulate real-world SOC investigation tasks such as monitoring VPN access, analyzing user activity, correlating IP addresses, and reviewing geographic access patterns.
VPN Log Investigation Report

 Analyst Role
SOC Level 1 Analyst

Tool Used
Elastic Stack – Kibana (Discover)

 SOC VPN Log Analysis Using Elastic Stack

Overview
This project demonstrates a SOC Level 1 investigation using Elastic Stack (Kibana Discover) to analyze VPN connection logs and identify high-activity users, source IPs, and abnormal traffic patterns.

 Tools Used
- Elastic Stack
- Kibana (Discover)

 Investigation Summary
VPN logs were analyzed by applying time filters, field-based filters, and histogram analysis to identify usage trends and investigate abnormal spikes in activity.

Key Investigation Steps
- Selected VPN index pattern
- Applied full time-range filtering
- Identified top source IPs and users
- Investigated VPN traffic spike on January 11
- Applied geographic exclusion filters

Key Skills
- SIEM log analysis
- Elastic / Kibana
- VPN traffic investigation
- SOC alert triage
 Field-based filtering

  screenshots
  ![IMG_1036](https://github.com/user-attachments/assets/cb6a35cc-8cf4-460f-89f9-b36faf83ebf6)
  User Activity Analysis
Reviewed VPN usage by username to identify users responsible for the highest VPN traffic. The analysis shows that one user generated the most VPN connections, which may indicate heavy remote usage or require further review depending on business context



![IMG_1039](https://github.com/user-attachments/assets/44137807-ba73-48c1-b961-e8a131bbaba2)

Geographic Filtering Analysis
Applied a filter to exclude connections originating from New York state for a specific source IP. This revealed 48 VPN connections from other locations, which could indicate travel, VPN misuse, or shared credentials.


![IMG_1035](https://github.com/user-attachments/assets/0de5503f-784a-4f25-98d5-a572adb45441)

Source IP Attribution (User-Focused)
Identified the source IP addresses associated with the user Emanda. IPs have been anonymized. One IP accounted for the majority of the user’s VPN connections, suggesting a consistent access location.

![IMG_1038](https://github.com/user-attachments/assets/0a1b8073-faea-4b12-a653-5bef4b00125a)
Anomaly Detection via Timeline Analysis
Identified a significant spike in VPN activity on January 11, 2022 using the time histogram. Further investigation showed that a single source IP was responsible for the increase in connections on that date.


![IMG_1032](https://github.com/user-attachments/assets/5a1d7f4a-ea4a-4301-88ea-719c7c2f4cd7)
User Activity Analysis
Reviewed VPN usage by username to identify users responsible for the highest VPN traffic. The analysis shows that one user generated the most VPN connections, which may indicate heavy remote usage or require further review depending on business context.





  
- Timeline and spike investigation
- SOC investigation workflow
