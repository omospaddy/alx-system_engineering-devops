Postmortem: Web Server Outage on June 1, 2024
Issue Summary:

Duration: June 1, 2024, 10:00 AM - June 1, 2024, 12:00 PM (UTC)
Impact: The web server hosting our company's website experienced an outage, rendering the website inaccessible to users. Approximately 75% of users were affected, experiencing either slow loading times or complete unavailability.
Root Cause: A misconfiguration in the server's firewall settings inadvertently blocked incoming traffic, causing the server to reject legitimate user requests.
Timeline:

10:00 AM: The issue was first detected when monitoring alerts indicated a sudden drop in server responsiveness.
10:05 AM: Engineers noticed an increase in customer complaints regarding slow website loading times.
10:10 AM: Initial investigation focused on the server's resource utilization and network connectivity.
10:30 AM: Assumptions were made that the issue might be due to high server load or network congestion.
10:45 AM: Further investigation revealed no abnormal resource usage or network issues.
11:00 AM: Escalation to the networking team as suspicions grew about a possible firewall misconfiguration.
11:30 AM: After thorough examination, it was confirmed that the firewall settings were blocking incoming traffic.
11:45 AM: Immediate action was taken to reconfigure the firewall to allow incoming traffic.
12:00 PM: The website was restored to full functionality as the firewall issue was resolved.
Root Cause and Resolution:

Root Cause: The root cause of the issue was identified as a misconfiguration in the server's firewall settings. The firewall was incorrectly configured to block incoming traffic, leading to the rejection of legitimate user requests.
Resolution: The issue was resolved by promptly reconfiguring the firewall to allow incoming traffic. Additionally, measures were put in place to ensure proper configuration management to prevent similar incidents in the future.
Corrective and Preventative Measures:

Improvements/Fixes:
Regular audits of firewall configurations to ensure alignment with security policies.
Implement automated monitoring for firewall rules to detect and alert on any unexpected changes.
Tasks:
Conduct a comprehensive review of all server firewall configurations to identify and correct any potential misconfigurations.
Develop and implement automated tests to verify the integrity of firewall rules after any configuration changes.
