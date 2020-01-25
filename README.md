# Sigma
Generic rule format for SIEM Solutions
Sigma is a generic and open signature format to detect malware and other security-related events in log files. Which are the log files currently supported? 

Firewall logs
Operating System logs
Proxy logs
Web server access logs

For Windows, the operating system logs include:

Sysmon events
Event logs 
Process creation events

Logs are usually kept in a security information and event management system (SIEM). To search in your SIEM or log source, Sigma offers to convert your rule into a search query specific to your SIEM product (the target):



<img>

Currently, Sigma rules can be converted to the following targets:


Splunk (plain queries and dashboards)
ElasticSearch Query Strings
ElasticSearch Query DSL
Kibana
Elastic X-Pack Watcher
Logpoint
Windows Defender Advanced Threat Protection (WDATP)
Azure Sentinel / Azure Log Analytics
Sumologic
ArcSight
QRadar
Qualys
RSA NetWitness
PowerShell
Grep


By supporting so many targets, Sigma has a tremendous advantage: one rule can be used in various SIEMs. This allows sharing, prevents vendor lock-in, and makes Sigma generic

#References
https://www.joesecurity.org/blog/8225577975210857708
https://github.com/Neo23x0/sigma
