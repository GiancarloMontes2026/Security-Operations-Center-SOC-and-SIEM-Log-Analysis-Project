# Splunk SIEM: Security Log Analysis, Threat Detection & Dashboards

## Overview

This project documents a hands-on **Blue Team Security Operations Center (SOC) lab** completed as part of CodePath's Intermediate Cybersecurity (CYB102) program.

The lab focused on using **Splunk Enterprise as a Security Information and Event Management (SIEM) platform** to search, analyze, and visualize data, investigate authentication events, and create dashboards and reports.

The primary objective was to develop practical experience with **SIEM operations, security log analysis, threat detection concepts, and data visualization**, demonstrating how SOC analysts use centralized logging platforms to investigate potentially suspicious activity.

## Lab Objectives

The primary objectives of this lab were to:

- Navigate and configure the Splunk Enterprise interface.
- Understand Splunk terminology including indexes, sourcetypes, sources, hosts, and timestamps.
- Build and execute searches to retrieve relevant events.
- Analyze datasets using Splunk Search Processing Language (SPL).
- Use statistical commands to identify patterns within data.
- Create visualizations to identify patterns and trends.
- Develop dashboards to organize and present information.
- Investigate Linux authentication logs for suspicious login activity.
- Identify source IP addresses associated with failed authentication attempts.
- Create reports summarizing security-relevant findings.

## Lab Environment & Tools

The lab was conducted in an **Ubuntu virtual machine** with a preconfigured Splunk Enterprise instance.

Tools and technologies used included:

- Splunk Enterprise
- Splunk Search & Reporting
- Splunk Search Processing Language (SPL)
- Ubuntu Linux
- Linux Authentication Logs (`auth.log`)
- Web Server Security Logs
- Data Visualization
- Splunk Dashboards
- Security Reporting

## Splunk Environment & Data Exploration

The investigation began by accessing **Splunk Enterprise** through the Ubuntu virtual machine.

I explored the Splunk interface and learned how its indexing and field structure supports efficient searches across large datasets.

Important Splunk components included:

- **Index** — Organizes searchable data.
- **Sourcetype** — Identifies the format or type of incoming data.
- **Source** — Identifies where the data originated.
- **Host** — Identifies the system associated with an event.
- **Time** — Provides timestamps used to analyze when events occurred.

Understanding these components established a foundation for locating, filtering, and investigating relevant events.

## Data Analysis & SPL Searches

The lab introduced Splunk's **Search & Reporting** application, which allows analysts to retrieve and analyze events from indexed datasets.

I practiced filtering information and using statistical commands to summarize results.

An example SPL search used during the lab was:

```spl
index=main host="WebServer01"
```

This search retrieves indexed events associated with the designated web server.

I also explored statistical commands such as:

```spl
stats
```

and:

```spl
count
```

These capabilities allow analysts to aggregate information, reduce large volumes of event data, and identify patterns that may require further investigation.

## Dashboards & Data Visualization

Another component of the lab involved creating **Splunk dashboards and visualizations**.

I practiced transforming search results into charts and organizing the resulting information into dashboard panels.

The exercises initially used a video game sales dataset to demonstrate statistical analysis and visualization before transitioning to security-focused log investigations.

Dashboards can help analysts:

- Monitor event activity.
- Identify unusual patterns.
- Visualize trends.
- Summarize large datasets.
- Organize investigation results.
- Communicate findings.

## Security Log Investigation

The final required exercise focused on analyzing **Linux authentication activity** from a web server.

The dataset contained records of successful and failed login attempts.

Using Splunk, I investigated authentication activity and examined source IP addresses associated with failed login attempts.

The investigation followed a workflow similar to:

**Authentication Logs → Splunk Search → Failed Login Events → Source IP Analysis → Investigation**

The objective was to understand how authentication logs can provide evidence of potentially unauthorized access attempts.

This exercise demonstrated how a SIEM can help security analysts efficiently search, filter, and analyze security events from monitored systems.

## Failed Authentication Analysis

Failed authentication events can provide useful indicators during a security investigation.

By examining authentication logs in Splunk, I was able to analyze login activity and identify source IP addresses associated with failed authentication attempts.

This demonstrated how analysts can use centralized logging to investigate authentication behavior and determine which events may require additional analysis.

## Security Reporting

The lab also introduced **Splunk reporting capabilities**.

Reports allow analysts to save searches, organize findings, and communicate security information in a consistent format.

I explored how reports can summarize authentication activity and support ongoing monitoring or additional investigation.

## SOC Analysis Workflow

The project demonstrated a fundamental SIEM investigation workflow:

**Collect Logs → Search Events → Filter Relevant Activity → Analyze Patterns → Investigate Suspicious Behavior → Visualize Findings → Generate Reports**

This workflow demonstrates how centralized logging platforms can help SOC analysts transform raw event data into information that supports security investigations.

## Skills Demonstrated

- Security Operations Center (SOC) Fundamentals
- SIEM Monitoring
- Splunk Enterprise
- Splunk Search Processing Language (SPL)
- Security Log Analysis
- Authentication Log Investigation
- Failed Login Analysis
- Source IP Analysis
- Threat Detection Concepts
- Linux Security
- Event Analysis
- Data Visualization
- Security Dashboards
- Security Reporting
- Blue Team Security

## Key Takeaways

This lab strengthened my understanding of how SOC analysts use **SIEM platforms to collect, search, analyze, and visualize security data**.

By investigating Linux authentication events in Splunk, I gained practical experience searching security logs, filtering events, identifying failed authentication activity, examining associated source IP addresses, and organizing findings through dashboards and reports.

The project also reinforced the importance of **centralized logging, event analysis, visualization, and security reporting** within modern Security Operations Center environments.

## Disclaimer

This project was completed in an **authorized educational lab environment** as part of CodePath's Intermediate Cybersecurity (CYB102) program.

All datasets, investigations, and activities were used for educational and cybersecurity training purposes.
