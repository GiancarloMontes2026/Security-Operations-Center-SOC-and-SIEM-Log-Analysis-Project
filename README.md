plunk SIEM: Security Log Analysis, Threat Detection & Dashboards

Overview

This project documents a hands-on Blue Team Security Operations Center (SOC) lab completed as part of CodePath's Intermediate Cybersecurity (CYB102) program.

The lab focused on using Splunk Enterprise as a Security Information and Event Management (SIEM) platform to search, analyze, and visualize data, investigate authentication events, and create dashboards and reports.

The primary objective was to develop practical experience with SIEM operations, security log analysis, threat detection, and data visualization, demonstrating how SOC analysts use centralized logging platforms to investigate potentially suspicious activity.

Lab Objectives

The primary objectives were to:

Navigate and configure the Splunk Enterprise interface.

Understand Splunk terminology, including indexes, sourcetypes, sources, hosts, and timestamps.

Build and execute searches to retrieve relevant events.

Analyze datasets using Splunk search commands.

Create visualizations to identify patterns and trends.

Develop dashboards to organize and present information.

Investigate Linux authentication logs for suspicious login activity.

Identify source IP addresses associated with failed authentication attempts.

Create reports summarizing security-relevant findings.

Lab Environment & Tools

The lab was conducted in an Ubuntu virtual machine with a preconfigured Splunk Enterprise instance.

Tools and technologies:

Splunk Enterprise

Splunk Search & Reporting

Splunk Search Processing Language (SPL)

Ubuntu Linux

Linux authentication logs (auth.log)

Web server security logs

Data visualization and dashboards

Security reporting

Splunk Environment & Data Exploration

The investigation began by accessing Splunk Enterprise through the Ubuntu virtual machine.

I explored the Splunk interface and learned how its indexing and field structure supports efficient searches across large datasets.

Important Splunk components included:

Index: Organizes searchable data.

Sourcetype: Identifies the format or type of incoming data.

Source: Identifies where the data originated.

Host: Identifies the system associated with an event.

Time: Provides timestamps for analyzing events.

Understanding these components helped establish a foundation for locating and investigating relevant events.

Data Analysis & SPL Searches

The lab introduced Splunk's Search & Reporting application, which allows analysts to retrieve and analyze events from indexed datasets.

I practiced filtering information and using statistical commands to summarize results.

Example SPL search:

index=main host="WebServer01"

This search retrieves indexed events associated with the designated web server.

I also explored statistical commands such as stats and count to aggregate information and identify patterns within datasets.

These capabilities are important for SOC investigations because they allow analysts to reduce large volumes of log data into meaningful information.

Dashboards & Data Visualization

Another component of the lab involved creating dashboards and visualizations using Splunk.

I explored how to transform search results into charts and organized dashboard panels.

The exercises initially used a video game sales dataset to demonstrate statistical analysis and visualization before transitioning to security-focused log investigations.

Dashboards can help security analysts:

Monitor event activity.

Identify unusual patterns.

Visualize trends.

Summarize large datasets.

Communicate investigation findings.

Security Log Investigation

The final required exercise focused on analyzing authentication activity from a Linux web server.

The dataset contained records of successful and failed login attempts.

Using Splunk, the investigation focused on identifying suspicious authentication behavior and examining source IP addresses associated with failed login activity.

The objective was to understand how authentication logs can provide evidence of potentially unauthorized access attempts.

This exercise demonstrated how SIEM platforms support security investigations by allowing analysts to search, filter, and analyze events from monitored systems.

Security Reporting

The lab also introduced Splunk reporting capabilities.

Reports allow analysts to save searches, organize findings, and communicate security information in a consistent format.

I explored how reports can summarize authentication activity and support ongoing monitoring or further investigation.

Skills Demonstrated

Security Operations Center (SOC) • SIEM Monitoring • Splunk Enterprise • Splunk SPL • Security Log Analysis • Authentication Log Investigation • Threat Detection Concepts • Linux Security • Failed Login Analysis • Data Visualization • Security Dashboards • Reporting • Blue Team Security

Key Takeaways

This lab strengthened my understanding of how SOC analysts use SIEM platforms to collect, search, analyze, and visualize security data.

The investigation followed a fundamental SOC workflow:

Collect logs → Search events → Filter relevant activity → Analyze patterns → Investigate suspicious behavior → Visualize findings → Generate reports

The project provided practical exposure to Splunk Enterprise and reinforced the importance of centralized logging, event analysis, and security reporting in modern cybersecurity operations.

Disclaimer

This project was completed in an authorized educational lab environment as part of CodePath's Intermediate Cybersecurity (CYB102) program.

All datasets, investigations, and activities were used for educational and cybersecurity training purposes.
